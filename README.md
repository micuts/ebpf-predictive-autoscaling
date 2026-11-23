# eBPF Predictive Autoscaling on K3s

## Kiến trúc hệ thống (Máy A - Cluster Host)
- **Kubernetes:** K3s (tắt Flannel, kube-proxy và Traefik mặc định)
- **CNI & eBPF Observability:** Cilium + Hubble (bật OpenMetrics & L7 HTTP policy)
- **Monitoring & Autoscaling:** Prometheus, Grafana, KEDA
- **Workload:** Google Online Boutique (namespace `demo`, NodePort `30080`)
