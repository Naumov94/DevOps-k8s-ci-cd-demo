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

```
git clone https://github.com/Naumov94/DevOps-k8s-ci-cd-demo.git
cd DevOps-k8s-ci-cd-demo/app
```

### 2. Run locally (without Docker)

```
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

📌 Next Steps
 Add Helm chart

 Deploy to Kubernetes cluster

 Add CI/CD with GitHub Actions

 Manage infrastructure with Terraform
