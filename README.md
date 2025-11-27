# MyApp - FastAPI Python GitHub Actions CI/CD Pipeline with Self-Hosted-Runner.

This is a small FastAPI Python application deployed locally on Minikube using Helm with a production-grade CI/CD pipeline running on GitHub Actions self-hosted runner.

## Features
- FastAPI web app
- Dockerized
- Helm deployment
- CI/CD with GitHub Actions
- SonarQube code quality
- Trivy vulnerability scanning 
- Monitoring with Prometheus/Grafana 

## How to run locally
1. Start Minikube: `minikube start`
2. Install Helm charts: `helm upgrade --install myapp ./charts/myapp`
3. Access the app:
   ```bash
   kubectl port-forward svc/myapp 8000:8000

Visit http://localhost:8000/
