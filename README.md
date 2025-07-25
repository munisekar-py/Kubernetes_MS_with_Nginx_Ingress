# Kubernetes NGINX Microservices with Ingress (Minikube)

This project sets up three microservices using custom NGINX containers deployed to a local Minikube cluster, with routing managed by a single Ingress resource.

---
## 🧑‍💻 Author

**Munisekar R S**  
DevOps Enthusiast | Cloud & Kubernetes Explorer

## 🧩 Microservices

- **Microservice 1:** `service1.local.com` → "Welcome to Microservice 1"
- **Microservice 2:** `service2.local.com` → "Hello from Microservice 2"
- **Microservice 3:** `service3.local.com` → "Greetings from Microservice 3"

---
## 📁 Project Structure
<pre>
<code>
├── k8s
│   ├── deployments.yaml
│   ├── ingress.yaml
│   └── services.yaml
├── README.md
├── service1
│   ├── Dockerfile
│   └── index.html
├── service2
│   ├── Dockerfile
│   └── index.html
└── service3
    ├── Dockerfile
    └── index.html
</code>
</pre>

## 🛠 Prerequisites

- Docker
- Minikube
- kubectl

---

## 🚀 Setup Instructions

### 1. Start Minikube and Enable Ingress
```bash
 minikube start
 minikube addons enable ingress

  ```
### **2.Supporting commands**
- `minikube ip`
-  Update local `/ect/hosts` file with `<minikube-ip>  service1.local.com service2.local.com service3.local.com`
-  Set `eval $(minikube docker-env)` before docker build
  

