# BlogHub - Full-Stack Blogging Platform

---

## 📌 Overview | 项目简介

BlogHub is a full-stack blogging platform built with SvelteKit (frontend) and Node.js (backend). It provides core blogging functionalities including article management, user authentication, and interactive features such as comments, likes, and subscriptions.

The system is designed with a RESTful API architecture and follows a clear separation between frontend and backend layers. It demonstrates practical experience in building scalable web applications, including API design, authentication mechanisms, and database interaction.
 
BlogHub 是一个基于 SvelteKit（前端）和 Node.js（后端）构建的全栈博客系统，提供文章管理、用户认证以及评论、点赞、订阅等交互功能。

系统采用 RESTful API 架构，实现前后端分离，体现了在接口设计、用户认证机制及数据库交互方面的工程实践能力。

---

## 🧱 Architecture | 系统架构

```text
Frontend (SvelteKit)
        ↓
Backend API (Node.js + Express)
        ↓
Database (SQLite)
````

The frontend communicates with backend services through RESTful APIs. The backend handles business logic, authentication, and database operations.

前端通过 RESTful API 与后端通信，后端负责业务逻辑处理、用户认证及数据库操作。

---

## 🚀 Features | 核心功能

### 🔐 Authentication | 用户认证

* User registration and login
* JWT-based authentication mechanism
* Secure password handling with bcrypt

### 📝 Content Management | 内容管理

* Create, edit, and delete articles
* Dynamic article rendering
* Tag-based categorization

### 💬 Interaction System | 交互系统

* Comment system for articles
* Like functionality with real-time count
* Subscription system between users
* Notification mechanism

### 🎨 UI & UX | 界面体验

* Responsive design
* Modular frontend components
* Smooth user interaction

---

## 📁 Project Structure | 项目结构

* `frontend/` - SvelteKit 前端应用（页面渲染与用户交互）
* `backend/` - Node.js + Express 后端 API 服务（业务逻辑处理）
* `admin-client/` - Java 管理端客户端

---

## 🛠️ Tech Stack | 技术栈

### Frontend

* SvelteKit
* JavaScript (ES6+)
* CSS3

### Backend

* Node.js
* Express.js
* SQLite3
* JWT Authentication
* bcrypt

---

## 🗄️ Database | 数据库设计

Database: SQLite (`backend/project-database.db`)

### Core Tables

* `Users` - 用户信息
* `Articles` - 文章内容
* `Comments` - 评论数据
* `Tags` - 标签管理
* `Likes` - 点赞记录
* `Subscriptions` - 用户订阅关系
* `Notifications` - 通知信息

---

## ⚙️ Getting Started | 本地运行

### 1️⃣ Start Backend

```bash
cd backend
npm install
npm run dev
```

Backend server: [http://localhost:3000](http://localhost:3000)

---

### 2️⃣ Start Frontend

```bash
cd frontend
npm install
npm run dev
```

Frontend application: [http://localhost:5173](http://localhost:5173)

---

## 🔌 API Design | 接口设计

### Article APIs

* `GET /api/articles`
* `GET /api/articles/:id`
* `POST /api/articles`
* `PATCH /api/articles/:id`
* `DELETE /api/articles/:id`

### User APIs

* `POST /api/login`
* `POST /api/register`

### Comment APIs

* `GET /api/comments/articles/:id`
* `POST /api/comments`
* `DELETE /api/comments/:id`

### Like APIs

* `POST /api/likes`
* `GET /api/likes/:id/count`
* `GET /api/likes/:id/status`

---

## 🔐 Environment Variables | 环境变量

### Backend (.env)

```env
PORT=3000
DB_FILENAME=project-database.db
DB_INIT_SCRIPT=src/sql/init-db.sql
FRONTEND_ORIGIN=http://localhost:5173
JWT_KEY=YOUR_SECRET_KEY
```

### Frontend (.env)

```env
PUBLIC_API_BASE_URL=http://localhost:3000/api
PUBLIC_IMAGES_URL=http://localhost:3000/images
```

---

## 📊 Project Status | 项目状态

* Backend API implemented ✔
* Database integration completed ✔
* Frontend and backend connected ✔
* Core features functional ✔

---

## 🎯 Highlights | 项目亮点


* RESTful API-based system with clear frontend-backend separation
* Full-stack implementation covering UI, API, and database layers
* Authentication system using JWT and secure password encryption
* Modular structure supporting future scalability


* 基于 RESTful API 的系统设计，前后端职责清晰
* 覆盖前端、后端与数据库的完整全栈实现
* 使用 JWT 实现用户认证，并结合 bcrypt 进行密码加密
* 模块化结构设计，具备良好的扩展性

---

## 📌 Future Improvements | 后续优化方向

* Improve error handling and logging
* Optimize API response performance
* Enhance frontend state management
* Introduce more advanced backend architecture

---

## 📄 License

MIT License

---