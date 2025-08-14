# MiniGram-Microservices

A **microservices-based social media backend** built with **Node.js, Express, MongoDB, Redis, and Docker**, demonstrating scalable architecture, containerized deployment, and modular development.

---

## 🔹 Project Overview

MiniGram Microservices is a backend system designed for a social media platform, implementing **microservices architecture** for better scalability and maintainability. Each service is responsible for a specific domain:

* **API Gateway**: Central entry point routing client requests to appropriate services.
* **Identity Service**: Handles user registration, authentication, and authorization using JWT.
* **Post Service**: Manages creation, retrieval, and deletion of posts.
* **Media Service**: Handles media uploads (images/videos) and retrieval.
* **Search Service**: Provides efficient search for users and posts.

---

## 🛠️ Tech Stack

* **Backend**: Node.js, Express.js
* **Database**: MongoDB
* **Caching & Pub/Sub**: Redis
* **Authentication**: JWT
* **Containerization**: Docker, Docker Compose
* **CI/CD**: GitHub Actions (`.github/workflows/deploy.yml`)

---

## 📂 Folder Structure

```
MiniGram-Microservices/
├─ .github/workflows/deploy.yml
├─ api-gateway/
├─ identity-service/
├─ media-service/
│  ├─ src/
│  ├─ Dockerfile
│  ├─ package.json
├─ post-service/
│  ├─ src/
│  ├─ Dockerfile
│  ├─ package.json
├─ search-service/
│  ├─ src/
│  ├─ Dockerfile
│  ├─ package.json
├─ .gitignore
├─ docker-compose.yml
└─ README.md
```

---

## ⚙️ Features

* User registration, login, and JWT-based authentication
* CRUD operations for posts
* Media upload and retrieval
* Search functionality for posts and users
* Scalable microservices architecture
* Dockerized deployment for each service

---

## 🚀 Setup & Installation

### Prerequisites

* [Docker](https://www.docker.com/get-started)
* [Node.js](https://nodejs.org/en/) (optional if running services locally)
* [MongoDB](https://www.mongodb.com/) (optional if running without Docker)

### Steps

1. Clone the repository:

```bash
git clone https://github.com/harsh6029sharma/MiniGram-Microservices.git
cd MiniGram-Microservices
```

2. Start all services using Docker Compose:

```bash
docker-compose up --build
```

3. Access services (default ports):

* API Gateway: `http://localhost:3000`
* Identity Service: `http://localhost:3001`
* Post Service: `http://localhost:3002`
* Media Service: `http://localhost:3003`
* Search Service: `http://localhost:3004`

4. Use Postman or any API client to interact with endpoints.

---

## 📄 API Endpoints

### Identity Service

* `POST /auth/register` → Register a user
* `POST /auth/login` → Login and get JWT token

### Post Service

* `POST /posts` → Create a post
* `GET /posts` → Fetch all posts
* `DELETE /posts/:id` → Delete a post

### Media Service

* `POST /media/upload` → Upload media files
* `GET /media/:id` → Retrieve media

### Search Service

* `GET /search/posts` → Search posts
* `GET /search/users` → Search users

---


## 🧪 Testing

```bash
npm install
npm test
```

---

## 🔐 Security

* JWT for authentication
* Environment variables managed in `.env` 
* Docker containers isolate each service

---
## 📞 Contact

Harsh Sharma – [harsh@example.com](mailto:harshsharmahs.798@gmail.com)

---
**Thank You** 

