# DevOps Demo Project

A complete DevOps pipeline demo featuring:

- Python Flask (simple web app)
- Docker (containerization)
- GitHub Actions (CI pipeline)
- Docker Hub (image registry)
- Kubernetes + Helm (deployment)
- Minikube (local cluster for testing)

---

## 🚀 Getting Started

### 1. Clone the repo

```bash
git clone https://github.com/Naumov94/DevOps-k8s-ci-cd-demo.git
cd DevOps-k8s-ci-cd-demo
```

2. Run Locally (without Docker)
```
pip install -r app/requirements.txt
python3 app/app.py
```
Visit: http://localhost:5000

3. Build & Run with Docker
 ```
 docker build -t flask-demo-app ./app
 docker run -p 5000:5000 flask-demo-app
 ```

4. CI/CD Pipeline
✅ Every push to main triggers:

Docker image build via GitHub Actions

Image is pushed to Docker Hub:
https://hub.docker.com/r/naumov94/flask-demo-app


5. Deploy to Kubernetes (via Helm + Minikube)
```
# Install chart
helm install flask-app ./flask-app

# OR upgrade after changes
helm upgrade flask-app ./flask-app
```
To access the app:
```
kubectl port-forward service/flask-app 8080:5000
```
Open in browser:
➡️ http://localhost:8080

✅ Result
```
Hello from Flask inside Docker + Kubernetes!
```

📌 Bonus Features (coming next)
 GitHub Actions → Auto-deploy to K8s

 Ingress + Domain routing

 Prometheus + Grafana for monitoring

 Terraform for infra provisioning


 🤝 Author
Naumov94 on GitHub











