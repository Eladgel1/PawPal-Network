# 🐾 PawPal Network - Backend

The backend service that powers the PawPal Network platform.

---

## 🌟 Overview

The backend is responsible for handling authentication, user management, and core application logic. It exposes a RESTful API that the frontend consumes and is designed to be simple, reliable, and easy to extend.

---

## 🌍 Live API

- Base URL: https://pawpal-network-backend.onrender.com
- Health Check: https://pawpal-network-backend.onrender.com/health

---

## 🧠 Responsibilities

- User registration and login
- Authentication and protected routes
- Database access and data persistence
- Application initialization and health monitoring

---

## ⚙️ Local Setup

### Prerequisites

- Node.js (LTS recommended)
- MongoDB Atlas account or local MongoDB

### Install

```bash
cd backend
npm install
```

---

## 🔐 Environment Variables

Create a .env file inside the backend directory.

Example:

```bash
NODE_ENV=development
PORT=3000

MONGO_URI=mongodb+srv://<user>:<password>@<cluster>/<database>

CORS_ORIGIN=http://localhost:4200

JWT_SECRET=your_secret_here
JWT_EXPIRES_IN=1d
```

Note:
- If the MongoDB password contains special characters, it must be URL‑encoded inside the connection string.

---

## ▶️ Running the Server

Development / Local:

```bash
- npm run start
```

The server will run on the port defined in the environment variables (or fallback to 3000).

---

## 🔎 Common Endpoints

- GET /health - service health check
- POST /register - create a new user
- POST /login - authenticate an existing user

---

## 🌐 CORS Configuration

The backend restricts access to approved origins. Ensure that the frontend URL is explicitly allowed in the CORS configuration, including correct casing and protocol.

---

## ☁️ Deployment (Render)

This service is deployed as a Render Web Service.

Typical configuration:

- Root Directory: backend
- Build Command: npm install
- Start Command: npm run start
- Environment Variables: configured via Render dashboard

---

## 🛡️ Security Notes

- Never commit .env files
- Rotate credentials if they were ever exposed
- Restrict database access by IP where possible

---

This backend serves as the foundation of the PawPal Network platform and is structured to support future feature expansion and improvements.

