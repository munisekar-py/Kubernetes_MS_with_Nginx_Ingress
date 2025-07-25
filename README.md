# Kubernetes NGINX Microservices with Ingress (Minikube)

This project sets up three microservices using custom NGINX containers deployed to a local Minikube cluster, with routing managed by a single Ingress resource.

---

## 🧩 Microservices

- **Microservice 1:** `service1.local.com` → "Welcome to Microservice 1"
- **Microservice 2:** `service2.local.com` → "Hello from Microservice 2"
- **Microservice 3:** `service3.local.com` → "Greetings from Microservice 3"

---

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

