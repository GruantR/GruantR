# 👋 Hi, I'm Ruslan Trafimovich

**Backend Developer | Node.js | PostgreSQL | REST API**

I build **scalable and secure backend systems** with a focus on clean architecture and real-world production practices.

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

**Backend:** Node.js | Express.js  
**Database:** PostgreSQL | Sequelize ORM (migrations/seed + transactions)  
**Auth & Security:** JWT (access + refresh) | bcrypt | HttpOnly cookies | RBAC-ready roles  
**Storage:** LocalStorage + S3Storage (MinIO) | StorageInterface  
**Tools:** Docker / docker-compose | Redis | Jest + Supertest | Swagger/OpenAPI | GitHub Actions  
**Practices:** Validation | Centralized error handling | Caching & rate limiting  

---

## 💡 What I Focus On

- Backend architecture and scalability  
- Secure authentication and authorization  
- Storage and cloud integrations  
- Writing clean, maintainable code  

---

## 📈 Currently Improving

- Unit & integration testing (Jest, Supertest)  
- API documentation (Swagger / OpenAPI)  
- Logging and monitoring  

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
