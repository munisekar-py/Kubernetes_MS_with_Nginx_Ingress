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
  

##

<img width="1356" height="100" alt="image" src="https://github.com/user-attachments/assets/15f1e258-9865-4b23-8cc6-68c1cf1aef79" />


#
<img width="648" height="137" alt="image" src="https://github.com/user-attachments/assets/afcb889e-067b-4b90-a9de-85b018f4178a" />

