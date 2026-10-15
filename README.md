# CortexAI 🤖

**An AI-powered productivity platform built with React, Node.js, and microservices.**

CortexAI brings AI chat, coding assistance, PDF processing, image analysis, AI search, and presentation generation together in one platform.

## ✨ Features

- 💬 AI Chat Assistant
- 💻 Coding Assistant
- 📄 PDF Processing and RAG
- 🖼️ Image Analysis
- 🔎 AI-Powered Search
- 📊 PowerPoint Generation
- 🔐 Firebase Authentication
- 💳 Razorpay Payment Integration
- ⚡ Redis Integration

## 🛠️ Tech Stack

- **Frontend:** React.js, Vite, JavaScript, CSS
- **Backend:** Node.js, Express.js
- **State Management:** Redux Toolkit
- **Database:** MongoDB
- **Caching:** Redis
- **AI:** LLMs, Embeddings, Vector Database
- **Integrations:** Firebase, Razorpay, AWS S3, Tavily
- **Infrastructure:** Docker, Docker Compose

## 🏗️ Architecture

```text
CortexAI/
├── frontend/
└── backend/
    ├── gateway/
    ├── services/
    │   ├── agent/
    │   ├── auth/
    │   ├── billing/
    │   └── chat/
    └── shared/
        └── redis/
```

## 🚀 Getting Started

### Prerequisites

Install [Node.js](https://nodejs.org/), [Git](https://git-scm.com/), and [Docker Desktop](https://www.docker.com/products/docker-desktop/).

### 1. Clone the repository

```bash
git clone https://github.com/mayank6386/CortexAI.git
cd CortexAI
```

### 2. Install dependencies

Run `npm install` in the `frontend`, `backend/gateway`, and each backend service directory.

### 3. Configure environment variables

Create the required `.env` files for the frontend and backend services. Add your own MongoDB URI, AI API keys, Firebase settings, and payment credentials as required by the code.

**Never commit real credentials or `.env` files to GitHub.**

### 4. Start Redis

```bash
cd backend
docker compose up -d
```

### 5. Start backend services

Open separate terminals for each service:

```bash
cd backend/gateway
npm run dev
```

```bash
cd backend/services/agent
npm run dev
```

Start the `auth`, `billing`, and `chat` services in separate terminals as well.

### 6. Start the frontend

```bash
cd frontend
npm run dev
```

Open the local URL displayed by Vite, usually `http://localhost:5173`.

> Configure all required environment variables, databases, ports, and service URLs before running the complete application.

## 🔒 Security

- Keep API keys and database credentials private.
- Use environment variables for secrets.
- Never commit private credentials to version control.

## 👨‍💻 Author

**Mayank Mishra**

- GitHub: [@mayank6386](https://github.com/mayank6386)
- LinkedIn: [Connect with me](https://www.linkedin.com/in/mayank25042004)

## 📄 License

No license has been added yet.
