# 👋 Hi, I'm Ruslan Trafimovich

**Backend · Node.js · PostgreSQL · MongoDB**

Backend developer (**junior+ / early mid-level**) — **Node.js**, **Express**, **REST** APIs. Main depth: **PostgreSQL** + **Sequelize** (migrations, transactions); **MongoDB** from earlier projects. Also: **JWT**, **Redis**, **Docker**, **Jest** (unit + **Supertest** where needed), **Swagger**, file uploads with **local + S3-compatible** storage. Other experience: **Telegram Bot API** next to REST, **express-validator**, **analytics-style** endpoints (aggregations, funnel-style metrics), **layered** error handling.

---

## 🚀 Featured project

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

**Core:** Node.js | Express | REST  
**SQL:** PostgreSQL | Sequelize (migrations, seeds, transactions)  
**NoSQL:** MongoDB (worked with in past projects)  
**Auth & security:** JWT (access + refresh) | bcrypt | HttpOnly cookies | RBAC-ready roles  
**Infra & data:** Redis · Docker / Compose · local + S3-compatible storage (MinIO)  
**Validation & errors:** express-validator · centralized / layered error handling  
**Quality:** Jest + Supertest | Swagger/OpenAPI | GitHub Actions  
**Integrations:** Telegram Bot API (polling / webhook-oriented setups)  
**How I work:** clear layers (routes → services → storage / domain logic), tests and docs aligned with behavior

---

## 💡 Focus

- Reliable APIs and clear module boundaries  
- Security basics: auth, roles, safe uploads  
- Tests and docs that match real behavior  

---

## 📍 Current focus

- **Upload pipeline:** **magic-byte / file-signature checks** with **Multer** so files match real content (not only extension or `Content-Type`).

---

## 📈 Next steps

- Better **logging & monitoring** in production-like setups  
- Learn **TypeScript** + **Nest.js** and **migrate the file-storage project** when it fits the learning path  

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

⭐ *Backend that is clear to read, test, and ship.*
