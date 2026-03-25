# 🚀 Microservices Platform with Spring Boot, Docker, Kubernetes & AWS

## 📌 Overview

This project implements a microservices-based architecture using **Spring Boot** and **Spring Cloud**, designed for cloud-native environments.

It includes containerization with **Docker**, orchestration with **Kubernetes**, and deployment in **AWS using ECS and EKS**.

---

## 🧱 Architecture

The system is composed of:

* **msvc-usuarios** → User management
* **msvc-cursos** → Course management
* **msvc-auth** → Authentication (OAuth2)
* **msvc-gateway** → API Gateway (Spring Cloud Gateway)

---

## ☁️ Cloud Deployment (AWS)

This project was deployed in AWS using two approaches:

### 🐳 ECS (Elastic Container Service)

* Containerized services deployed using Docker
* Managed container orchestration without Kubernetes
* Suitable for simpler deployments

### ☸️ EKS (Elastic Kubernetes Service)

* Full Kubernetes cluster deployment
* Uses manifests (`deployment`, `service`, `configmap`, `secrets`)
* Demonstrates scalable cloud-native architecture

---

## 🐳 Docker

Run locally with Docker:

```bash
docker-compose up --build
```

---

## ☸️ Kubernetes

Deploy using:

```bash
kubectl apply -f .
```

Includes:

* Deployments
* Services
* ConfigMaps
* Persistent Volumes (MySQL/Postgres)

---

## 🔐 Security

* OAuth2 authentication implemented
* Spring Security for endpoint protection
* Secure inter-service communication

---

## ⚙️ Tech Stack

* Java 17
* Spring Boot
* Spring Cloud
* Spring Security (OAuth2)
* Spring Data JPA
* MySQL / PostgreSQL
* Docker
* Kubernetes
* AWS (ECS, EKS)

---

## 🚀 Build

```bash
mvn clean install -DskipTests
```

---

## 📡 Example Endpoints

* `GET /api/usuarios`
* `POST /api/auth/login`
* `GET /api/cursos`

---

## 🧠 Key Concepts

* Microservices architecture
* API Gateway pattern
* Service-to-service communication (Feign)
* Containerization (Docker)
* Orchestration (Kubernetes)
* Cloud deployment (AWS ECS & EKS)

---

## 📌 Notes

Originally based on a training course, this project was refactored and extended to demonstrate real-world backend and cloud engineering practices.

---

## 👨‍💻 Author

Developed and adapted by **Freyder**
