
# 🧠 AI-Powered Project Management Dashboard (Gantt Dashboard)


## 🚀 Project Overview

**AI-Powered Project Management Dashboard** is a full-stack platform designed to simplify project tracking and scheduling using dynamic **Gantt charts**.
It helps project managers define tasks, assign users, and visualize progress in real time.

The key differentiator is the built-in **Artificial Intelligence module**, which provides intelligent suggestions for task scheduling and resource optimization.
Everything is fully **containerized** with Docker, allowing you to run the entire stack using just one command.



## ✨ Key Features

* 📊 **Dynamic Gantt Chart:** Real-time visualization of project tasks, dependencies, and timelines.
* 🧩 **Comprehensive Admin Panel:** Manage users, tasks, and reports with full CRUD functionality.
* 🤖 **AI Integration:** Smart recommendations for task prioritization and workload balancing.
* 🌐 **Bilingual Support (EN/FA):** Seamlessly switch between English and Persian interfaces.
* 🔐 **Secure Authentication:** JWT-based session management for both users and admins.
* 🧾 **Interactive API Documentation:** Swagger-based OpenAPI interface for easy testing.
* 🐳 **Fully Containerized:** One-command deployment with `docker-compose` for all services.



## 💻 Technology Stack

| Layer                 | Technologies           |
| :-------------------- | :--------------------- |
| **Front-end**         | React.js, Tailwind CSS |
| **Back-end**          | Node.js, Express.js    |
| **Database**          | MongoDB                |
| **API Documentation** | Swagger / OpenAPI      |
| **Reverse Proxy**     | Nginx                  |
| **Containerization**  | Docker, Docker Compose |



## 🏛️ Project Architecture

The project follows a **multi-service architecture** managed via `docker-compose`.
**Nginx** serves as the **main gateway**, routing user requests to the appropriate service.

### 🔁 Request Flow

```
User
 └──> Nginx (Port 80)
       ├──> / → React Front-end (client)
       └──> /api → Node.js Back-end (server)
                     └──> MongoDB (database)
```

### 📦 Services

1. **Nginx:** Reverse proxy routing frontend and backend traffic.
2. **Client:** React-based web app providing the Gantt chart interface and admin panel.
3. **Server:** Node.js API handling business logic, AI modules, and data processing.
4. **MongoDB:** Database layer for storing users, tasks, and project reports.



## 🛠️ Getting Started

### Prerequisites

Make sure you have **Docker** and **Docker Compose** installed on your system.

### 1️⃣ Clone the repository

```bash
git clone https://github.com/your-username/ai-gantt-dashboard.git
cd ai-gantt-dashboard
```

### 2️⃣ Start the application

```bash
docker-compose up -d
```

Once the containers are up, access the dashboard at:
👉 [http://localhost](http://localhost)



## 📡 API Documentation

The interactive Swagger API docs are available at:

```
http://localhost/api/docs
```



## 🧩 Directory Structure

```
├── client/              # React frontend application
├── server/              # Express backend and AI modules
├── nginx/               # Reverse proxy configuration
├── docker-compose.yml   # Service definitions
└── README.md
```



## 📘 License

This project is released under the **MIT License**.
Please credit the authors if you use or modify this code. 💙