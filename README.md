# 🚀 The One-Month Backend Mastery Roadmap (Node.js/Express/SQL)

A **30-day guided project** to master backend development with **Node.js, Express, and SQL (PostgreSQL)**.  
This roadmap takes you from building a simple REST API → to authentication, security, testing, deployment, and advanced backend concepts.  

The final result: a **production-ready backend API** with users, projects, and tasks, following industry best practices.

---

## 📌 Project Goals
- Gain **strong backend fundamentals** without shortcuts.  
- Master **raw SQL** before moving to ORMs.  
- Learn to **design APIs, handle security, and deploy apps**.  
- Build a **portfolio project** you can showcase to employers.  

---

## 🛠️ Tech Stack
- **Node.js** (runtime)
- **Express.js** (backend framework)
- **PostgreSQL** (database)
- **pg (node-postgres)** (DB driver)
- **bcryptjs** (password hashing)
- **jsonwebtoken (JWT)** (authentication)
- **dotenv** (environment variables)
- **Joi / Zod** (validation)
- **Jest + Supertest** (testing)
- **Helmet, CORS, Morgan/Winston** (security, logging)
- **Render / Railway** (deployment)

---

## 📂 Project Structure
```bash
Task-Management-API/
├── controllers/        # Business logic for routes
│   └── projectController.js
├── db/                 # Database connection
│   └── index.js
├── routes/             # Express route definitions
│   └── projectRoutes.js
├── tests/              # Jest & Supertest tests
├── .env.example        # Example environment file
├── app.js              # Main app entry
├── package.json
└── README.md
```
---
## 🚦 Getting Started
**1️⃣ Prerequisites**
-Install Node.js (>= 18.x)
-Install PostgreSQL (>= 14.x)
-Create a new database:
```bash
CREATE DATABASE backend_mastery;
```
**2️⃣ Clone & Install**
```bash
git clone https://github.com/Hamza-Rafique/Task-Management-API
cdTask-Management-API
npm install
```
**3️⃣ Configure Environment**
Create a .env file in the project root:
```bash
PORT=5000
DATABASE_URL=postgresql://username:password@localhost:5432/Task-Management
JWT_SECRET=supersecretkey
```

**4️⃣ Run the Server**
```
bash npm run dev
```
Visit: http://localhost:5000/api/status

---
## 🔑 API Endpoints
**Health Check**
```bash
GET /api/status
```
Response:
```bash
{ "status": "OK" }
```
**User Authentication**

- **POST /api/users/register** → Register new user
- **POST /api/users/login** → Login and receive JWT
---
**Projects**

- **POST /api/projects** → Create project (🔒 requires JWT)
- **GET /api/projects** → Get all projects (for logged-in user)
- **GET /api/projects/:id** → Get single project
- **PUT /api/projects/:id** → Update project
- **DELETE /api/projects/:id** → Delete project
---
**Tasks**

- **GET /api/tasks** → Supports filtering, sorting, pagination
- **POST /api/tasks** → Create task under project
- **GET /api/tasks/:id** → Get task details
---
 ## 🧪 Testing
 Run API tests:
 ```bash
npm test
```
---
## 🚀 Deployment

- 1.Push code to GitHub.
- 2.Deploy on Render.com or Railway.app.
- 3.Add PostgreSQL instance and set environment variables.
 ---
 ## 🎯 Week-by-Week Roadmap
**Week 1: Core Fundamentals**

- Node.js & Express setup
- SQL basics & schema design
- CRUD APIs with raw SQL
- Data validation & error handling

**Week 2: Security & Authentication**

- Password hashing (bcrypt)
- JWT authentication & authorization middleware
- SQL relationships (Users ↔ Projects ↔ Tasks)
- Environment variables

**Week 3: Advanced Features**

- Pagination, filtering, sorting
- Unit & integration tests
- Logging & monitoring
- Deployment (Render/Railway)

**Week 4: Specialization (Pick One)**

- Option A: Database Performance
- Option B: Advanced Authentication (OAuth2, RBAC, refresh tokens)
- Option C: Docker & CI/CD pipeline
---
## 🌟 Final Advice

- **TypeScript**: For professional mastery, restart the project with TypeScript.
- **Read Open Source Cod**e: Explore real-world Express apps on GitHub.
- **Commit Daily**: Document your learning journey on GitHub.

**📜 License**

This project is open-source under the MIT License

