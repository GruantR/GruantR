# 👋 Hi, I'm Ruslan Trafimovich

**Backend Developer** — Node.js · Express · PostgreSQL · REST APIs · Docker

I ship **REST backends** with layered architecture: **PostgreSQL + Sequelize** (migrations, seeds, transactions), **JWT** (access/refresh, HttpOnly cookies) with **Redis** for caching, rate limiting, and token flows, and **object storage** (local + **S3-compatible MinIO**). I pair that with **Jest + Supertest**, **Swagger/OpenAPI**, **GitHub Actions** CI, and production-minded practices: validation, RBAC-ready roles, centralized errors, and Docker-first deployment.

---

## 🚀 Featured Project

### 📦 [File Storage Service](https://github.com/GruantR/file-storage-service)

Production-ready backend API for uploading, storing, and managing files with support for **local storage and S3-compatible cloud (MinIO)**.

**Key Features:**
- Pluggable storage drivers via `StorageInterface` (`LocalStorage` + `S3Storage`)
- Storage selection per upload (`storage=local|s3`) with correct read/delete routing via DB `storageType`
- JWT auth with refresh token rotation stored in PostgreSQL and mirrored in Redis (HttpOnly cookies)
- Secure uploads: Multer validation (types + size limits) and RBAC-ready user/admin roles
- Sequelize migrations + seed and transaction-safe deletion with cleanup logs
- Redis rate limiting + caching for list endpoints
- Swagger/OpenAPI docs and connectivity-first `/api/health`
- Docker-first setup + GitHub Actions smoke test

UI note: the demo front-end was built with AI assistance; the backend implementation was done independently.

---

## 🛠️ Tech Stack

**Runtime & API:** Node.js | Express.js | REST  
**Data:** PostgreSQL | Sequelize ORM (migrations, seeds, transactions)  
**Auth & security:** JWT (access + refresh) | bcrypt | HttpOnly cookies | RBAC-ready roles  
**Caching & limits:** Redis (cache, rate limiting, refresh-token flow)  
**Storage:** Local + S3-compatible (MinIO) via `StorageInterface`  
**Quality & ops:** Jest + Supertest | Swagger/OpenAPI | Docker / Compose | GitHub Actions  
**Practices:** Validation | Centralized error handling | layered modules (routes → services → storage)  

---

## 💡 What I Focus On

- Backend architecture and scalability  
- Secure authentication and authorization  
- Storage and cloud integrations  
- Clean, testable code aligned with how the system runs in production  

---

## 📍 Current focus

- **Upload hardening:** integrating **file signature (magic-byte) checks** with **Multer** so uploads match real content—not only declared extension or `Content-Type`—reducing **extension spoofing** and **MIME spoofing** risk.

---

## 📈 Roadmap

- **Observability:** structured logging and monitoring in real deployments  
- **Stack evolution:** deepening **TypeScript** and **Nest.js** with the goal of **rewriting the file-storage project** on that stack for clearer modules, typing, and maintainability at scale  

---

## 📊 Development Activity

### 💻 Codewars

[![Codewars](https://www.codewars.com/users/GruantRus/badges/large)](https://www.codewars.com/users/GruantRus)

### 📈 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=GruantR&show_icons=true&hide_border=true" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=GruantR&layout=compact&hide_border=true" />
</p>

---

## 📫 Contact

- LinkedIn: https://www.linkedin.com/in/ruslan-trafimovich-6a16b839a  
- Email: rusworv@gmail.com  
- GitHub: https://github.com/GruantR  

---

⭐ *Building backend systems that are not just working — but scalable and production-ready.*
