
[[Basic Requirements for Kubernetes in Production|Visual Diagram]]


**1 - Infrastructure as Code (IaC)**

First of all, managing your cloud infrastructure using Desired State configuration (Infrastructure as Code - IaC) comes with a lot of benefits and is a general cloud infrastructure best practice. Specifying it declaratively _as code_ will enable you to test your infrastructure (changes) in non-production environments. It discourages or prevents manual deployments, making your infrastructure deployments more consistent, reliable and repeatable. Teams implementing IaC deliver more stable environments rapidly and at scale. IaC tools like [Terraform](https://www.terraform.io/) or [Pulumi](https://www.pulumi.com/) work great to deploy your entire Kubernetes cluster in your cloud of choice together with networking, load balancers, DNS configuration and of course an integrated Container Registry. In our case, we use [Crossplane](https://www.crossplane.io/) for our IaC tool.

  

**2 - Monitoring & Centralized Observability (e.g Logs, Metrics, Traces, and Continuous Profiling)**

Kubernetes is a very stable platform. Its self-healing capabilities will solve many issues and if you don't know where to look you wouldn't even notice. However, that does not mean monitoring is unimportant. I have seen teams running production without proper monitoring, and suddenly a certificate expired, or a node memory overcommit caused an outage. You can easily prevent these failures with proper monitoring in place. [Prometheus](https://prometheus.io/) and [Grafana](https://grafana.com/) are Kubernetes' most used monitoring solutions and can be used to monitor _both your platform and applications_. Alerting (e.g. using an Alertmanager) should be set up for critical issues with your Kubernetes cluster, so that you can prevent downtime, failures or even data loss.

In addition, it is also important to run centralized components like [OpenTelemetry](https://opentelemetry.io/docs/) and [Grafana Agent ](https://grafana.com/docs/agent/latest/) to collect logging and send them to a centralized logging platform like [Loki](https://grafana.com/oss/loki/), metrics platform like [Mimir](https://grafana.com/oss/mimir/), traces platform like [Tempo](https://grafana.com/oss/tempo/), and continuous profiling platform like [Pyroscope](https://pyroscope.io/), so that application telemetry data can be centrally stored and accessed. These tools are configured such that standard monitoring is automatically in place for all apps without developer effort.


**3 - Centralized Ingress Controller with SSL certificate management**

(we do TLS/SSL termination at the edge via NGINX)

Kubernetes has a concept of Ingress. A simple configuration that describes how traffic should flow from outside of Kubernetes to your application. A central Ingress Controller (e.g. Nginx, Cilium, etc.) can be installed in the cluster to manage all incoming traffic for every application. When an Ingress Controller is linked to a public Cloud LoadBalancer (or self-hosted LB), all traffic is automatically load-balanced among Nodes, and sent to the intended pods' IP Addresses.

A Ingress Controller provides many benefits, because of its Centralization. It can also take care of HTTPS and SSL. An integrated component called cert-manager is a centrally deployed application in Kubernetes that takes care of HTTPS certificates. It can be configured using Let's Encrypt, wildcard certificates or even a private Certification Authority for internal company-trusted certificates. All incoming traffic will be automatically encrypted using the HTTPS certificates and forwarded to the correct Kubernetes pods. Another thing developers won't need to worry about.

  

**4 - Role-Based Access Control (RBAC)**

Not everyone should be a Kubernetes Administrator. We should always apply the principle of Least Privilege when it comes to Kubernetes access. Role-Based Access Control should be applied to the whole Kubernetes stack (Kubernetes API, deployment tools, dashboards, etc.). When we integrate Kubernetes with an IAM solution like Keycloak, Azure AD or AWS Cognito, we can centrally manage authentication and authorization using OAuth2 / OIDC for both platform tools and applications. Roles and groups can be defined to give users access to the resources they need to access based on their team or role.

  

**5 - GitOps Deployments**

Everyone who works with Kubernetes uses _kubectl_ one way or another. But manually deploying to Kubernetes using the 'kubectl apply' command is not a best practice, most certainly not in production. Kubernetes desired state configuration should be present in GIT, and we need a deployment platform that rolls out to Kubernetes. [ArgoCD](https://argo-cd.readthedocs.io/en/stable/) and [Flux](https://fluxcd.io/) are the two leading GitOps platforms for Kubernetes deployments. Both work very well for handling real-time declarative state management, making sure that Git is the single source of truth for the Kubernetes state. Even if a rogue developer tries to manually change something in production, the GitOps platform will immediately roll back the change to the desired change. With a GitOps bootstrapping technique we can manage environments, teams, projects, roles, policies, namespaces, clusters, appgroups and applications. With Git only. GitOps makes sure that all changes to all Kubernetes environments are 100% traceable, easily automated and manageable.

  

**6 - Secret Management**

Kubernetes secret manifests are used to inject secrets into your containers, either as environment variables or file mappings. Preferably, not everyone should be able to access all secrets, especially in production. Using Role-Based Access Control on secrets for team members and applications is a security best practice. Secrets can be injected into Kubernetes using a CI / CD tooling or (worse) via a local development environment, but this can result in configuration state drift. This is not traceable, and not easily manageable. The best way to sync secrets is using a central vault, like Azure Key Vault, Hashicorp Vault, AWS Secrets Manager with a central secrets operator like [External Secrets Operator](https://external-secrets.io/). This way, secret references can be stored in GIT, pointing to an entry in an external secrets Vault. For more security-focused companies it is also an option to lock out all developers from secrets in Kubernetes using RBAC. They will be able to reference secrets, and use them in containers, but will never be able to directly access them.

  

**Conclusion**

It is very important to have a good Infrastructure as Code solution, proper monitoring, RBAC and Deployment mechanisms that are secure, manageable and traceable. The earlier, the better. Setting up your Kubernetes cluster according to best practices using standardized open source tooling will help you save time, failures and headaches, especially in the long run. Of course, these are the most basic requirements for your Kubernetes stack, especially for enterprise-level companies. Other important considerations that have not been mentioned are ServiceMesh, Security scanning / compliance, end-to-end traceability, which will be discussed elsewhere.