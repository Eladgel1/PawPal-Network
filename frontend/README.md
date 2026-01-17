# 🐾 PawPal Network - Frontend

The web client for PawPal Network platform.

---

## 🌟 Overview

The frontend provides the user‑facing experience of PawPal Network. It focuses on clear navigation, smooth user flows, and a friendly interface that allows pet owners to interact with the platform effortlessly.

---

## 🌍 Live Application

- Web App: https://pawpal-network-frontend.onrender.com
- Backend API: https://pawpal-network-backend.onrender.com

---

## 🧠 Features

- User registration and login
- Client‑side routing and navigation
- Integration with the backend API
- Clean and responsive UI structure

---

## ⚙️ Local Setup

### Prerequisites

- Node.js (LTS recommended)

### Install

```bash
cd frontend
npm install
```

---

## ▶️ Run Locally

Start the development server:

```bash
npm run start
```

The application will be available locally (default Angular port).

If a proxy configuration is used, ensure it points to the local backend server.

---

## 🔧 API Configuration

The frontend communicates with the backend via a configured API base URL. For production, requests are sent to:

- https://pawpal-network-backend.onrender.com

Ensure this value is aligned with your environment or proxy configuration.

---

## ☁️ Deployment (Render)

The frontend is deployed as a static site on Render.

Typical configuration:

- Root Directory: frontend
- Build Command: npm install && npm run build
- Publish Directory: dist/<project-name>/browser

If you encounter a "Not Found" page after deployment, double‑check the publish directory path produced by the Angular build.

---

## 🎨 UI & UX Notes

- The project is structured for clarity and maintainability
- Components and pages are organized to support future feature growth
- Styling and layout are designed with simplicity and readability in mind

---

This frontend completes the PawPal Network experience by delivering a smooth, accessible interface for end users.

