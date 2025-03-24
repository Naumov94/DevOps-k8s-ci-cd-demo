# DevOps Demo Project

This is a full DevOps pipeline demo using:

- Python Flask (simple web app)
- Docker
- Kubernetes with Helm *(coming next)*
- CI/CD via GitHub Actions *(coming soon)*
- Infrastructure as Code with Terraform *(later)*
- Optional: Monitoring with Prometheus & Grafana

---

## 🚀 Getting Started

### 1. Clone the project

```bash
git clone https://github.com/Naumov94/DevOps-k8s-ci-cd-demo.git
cd DevOps-k8s-ci-cd-demo/app
```

### 2. Run locally (without Docker)

```bash
pip install -r requirements.txt
python3 app.py
```
Visit: http://localhost:5000

### 3. Build and run with Docker

```
docker build -t flask-demo-app .
docker run -p 5000:5000 flask-demo-app
```

## ✅ Result

The app will respond with:

```
Hello from Flask inside Docker + Kubernetes!
```


🪖 Deploy with Helm (Template Preview Only)

You can generate Kubernetes manifests using this Helm chart without applying anything:

```bash
cd app
helm template flask-app
```

This will render the actual deployment and service configuration based on values.yaml.



## 📌 Next Steps

✅ Add Helm chart  
🔜 Deploy to Kubernetes cluster  
🔜 Add CI/CD with GitHub Actions  
🔜 Manage infrastructure with Terraform
