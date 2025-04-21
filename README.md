# 📡 EKS Cluster Monitoring with Prometheus & Grafana

This project sets up a complete monitoring solution on an AWS EKS cluster using **Prometheus**, **Grafana**, and **Kube-State-Metrics**. It provides production-ready visibility into workloads, pods, services, nodes, and cluster health.

---

## 🔍 Features

- Kubernetes-native Prometheus deployment
- Grafana dashboards for cluster observability
- Helm support or raw manifests
- Alertmanager integration
- Kube-State-Metrics for advanced workload insights

---

## 📦 Tech Stack

- AWS EKS
- Kubernetes
- Prometheus
- Grafana
- Helm (optional)
- Kube-State-Metrics
- Alertmanager

---

## 🗂️ Project Structure

```text
eks-cluster-monitoring/
├── prometheus/            # Prometheus deployment and config
├── grafana/               # Grafana setup with dashboards and data sources
├── alertmanager/          # Alertmanager configs
├── kube-state-metrics/    # Resource metrics service
├── dashboards/            # JSON dashboard templates
├── helm/                  # Optional Helm chart overrides
├── README.md              # Project documentation
└── LICENSE                # MIT License

🚀 Getting Started
Prerequisites
AWS EKS cluster (running)

kubectl configured

Helm (optional)

📥 Installation (Using kubectl)
Deploy kube-state-metrics:
kubectl apply -f kube-state-metrics/

Deploy Prometheus:
kubectl apply -f prometheus/
Deploy Grafana:
kubectl apply -f grafana/

Set up Alertmanager:
kubectl apply -f alertmanager/

🎯 Access Grafana
kubectl port-forward svc/grafana 3000:3000
Visit http://localhost:3000 (Default login: admin / admin)

📊 Dashboards
Includes prebuilt Grafana dashboards for:

Node & Pod metrics

Cluster health overview

Kubernetes resource usage

🤝 Contributing
Contributions are welcome. Fork the repo and submit a PR!

📄 License
Licensed under the MIT License.

👤 Author
Lavanya J
📧 lavanyaj365@gmail.com
🔗 LinkedIn
🔗 GitHub
