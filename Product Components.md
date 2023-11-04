
# Table of Contents:

- External Load Balancer
- Internal Developer Platform
- Website
- CLI
- Billing Service
- Email Service (invoices, newsletters, updates to ToS, etc.)

---
### External Load Balancer:

Deployed as multiple containers within the same Autoscaling Group nodes, our self hosted configuration for a Highly-Available and Multi-Geo load balancer located behind AWS Route53 is as follows:

A. NGINX
B. HAProxy
C. Keepalived

NGINX is responsible for TLS/SSL termination, handing off unencrypted traffic to HAProxy to Load Balance to Kubernetes clusters (2 environments (dev & prod) per region), or to the company website (isomorphic SvelteKit application).

---
# Internal Developer Platform

##### Ideal Tech Stack:
- ytt
- Tanka
- Redis
- PostgreSQL
- Docker & Containerd
- Kubernetes
- K3s (or kind)
- Rancher Desktop (or Docker Desktop):
- ArgoCD
- Tekton
- KubeVela
- Crossplane
- Packer
- Cilium
- Hubble
- Falco (+ Falco Sidekick)
- Vault
- Teleport
- Telepresence
- Harbor
- Dragonfly
- Cert-Manager
- OpenTelemetry
- Grafana
- Grafana Agent (flow mode)
- Prometheus (+ exporters)
- Loki
- Mimir
- Tempo
- Pyroscope
- Alertmanager
- Capsule
- Vcluster
- Kyverno
- Kubescape
- Karpenter
- Velero
- Rook (ceph-operator)
- k6
- ChaosMesh
- KEDA
- SysDig
- Inspektor Gadget
- Tracee
- Kured
- Telepresence
- kube-iptables-tailer

+

- Rclone
- Kafka


---

# Website

##### Tech Stack:
- SvelteKit
- TailwindCSS

---

### CLI Tool

Written in Go using the Cobra library


--- 

# Billing Service

Built using Lago (+ Stripe)

---

# Email Service

ideally self-hosted using a solution such as MailCow. It would drastically reduce the monthly bill instead of a managed solution like gmail, but either is fine.