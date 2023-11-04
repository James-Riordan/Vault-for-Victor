
1. User Request:
   - CRUD requests via CLI or Website UI

2. AWS Route53:
   - Global Server Load Balancer directing traffic to the nearest NGINX & HAProxy instance

3. NGINX & HAProxy:
   - NGINX performs TLS/SSL termination.
   - Unencrypted traffic is then handed off to HAProxy (running in a different container within the same Autoscaling Group Nodes).
   - HAProxy load balances traffic to Kubernetes clusters.

4a. Cilium Ingress Controller:
   - Cilium Service Mesh controls and routes traffic to relevant pods.

4b. (optional) API Gateway:
   - Optional component for additional API management.

5. Cilium Service Mesh:
   - Responsible for routing and managing traffic to the specific pods within your Kubernetes clusters.