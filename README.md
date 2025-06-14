# Note-GPT
# 🤖 AI SaaS Chatbot – Full-Stack GPT-based Assistant (MERN + TypeScript)

Welcome to the AI SaaS Chatbot project! This is a **full-stack, production-ready, secure, and scalable** AI chatbot web application inspired by ChatGPT. Built with **TypeScript** and the **MERN (MongoDB, Express, React, Node.js)** stack, it integrates OpenAI's GPT-3.5/4 to deliver intelligent, real-time conversations via a sleek modern UI.

## 🚀 Demo
---
![Screenshot 2025-06-14 235210](https://github.com/user-attachments/assets/85186aa8-edc4-4939-8969-65fbfccc4d44)

---
![Screenshot 2025-06-14 232844](https://github.com/user-attachments/assets/358b8ed2-5f8e-4791-9333-0c5b99d1c291)

---
![Screenshot 2025-06-14 232513](https://github.com/user-attachments/assets/2bcc2bd2-5975-4eca-aaaa-3094be2fd33b)

---
![Screenshot 2025-06-14 233005](https://github.com/user-attachments/assets/9cf42047-d56a-4c2b-a1cb-3eaab03ffa62)

---
![Screenshot 2025-06-14 232556](https://github.com/user-attachments/assets/cd92f6db-05ab-4923-93e6-b2630f0eecac)

---


## 🧰 Tech Stack

- **Frontend:** React (with Context API & Material UI)
- **Backend:** Node.js, Express.js, TypeScript
- **Database:** MongoDB (Mongoose ODM)
- **Authentication:** JWT (JSON Web Tokens), Bcrypt, HTTP-only Cookies
- **AI Integration:** OpenAI GPT-3.5 & GPT-4 (via OpenAI API)
- **Dev Tools:** Morgan, dotenv, concurrently, nodemon, ts-node

---

## 🧠 Features

- ✨ **ChatGPT-like experience** – Ask coding questions, get formatted responses with code blocks.
- 🔐 **Secure login & session management** – HTTP-only cookies, JWT, 7-day token lifetime.
- 🧾 **Chat history persistence** – Chats stored in MongoDB, retrievable on session reload.
- 🧹 **Conversation management** – Clear all conversations with one click.
- 📱 **Responsive design** – Fully optimized UI for all devices.
- 🔄 **Session retention** – Seamless login experience maintained for 7 days.
- 🧩 **Modular & scalable architecture** – Separate routes, controllers, models, and utils.

---

## 📁 Project Structure

```bash
/client          → Frontend React app
/server          → Backend Node/Express API (TypeScript)
│
├── /src
│   ├── /controllers     → Route handler logic
│   ├── /models          → Mongoose schemas (User, Chat, etc.)
│   ├── /routes          → Express route definitions
│   ├── /middlewares     → Auth, validation, error handling
│   ├── /config          → DB, environment setup
│   └── /utils           → Helper functions/utilities



---

## 🔐 Authentication & Security

- Passwords are hashed using **bcrypt**.
- Sessions are authenticated via **JWT** stored in **HTTP-only cookies**.
- Security best practices with **environment variables** and API key management.

---

## 📡 OpenAI Integration

- Utilizes **Chat Completion API** from OpenAI.
- Supports **GPT-3.5-turbo** and **GPT-4**.
- Built-in support for code blocks, multi-turn conversations, and role (user/assistant) messages.

---

## 🛠️ Getting Started

### Prerequisites

- Node.js v18+
- MongoDB Atlas or Local Instance
- OpenAI API Key

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/ai-saas-chatbot.git
cd ai-saas-chatbot

### Backend setup
cd server
cp .env.example .env # Create your environment file
npm install
npm run dev

### Frontend setup
cd client
npm install
npm run dev

### Environment Variables
Create a .env file in /server with:

env
PORT=5000
MONGODB_URL=your_mongo_connection
JWT_SECRET=your_jwt_secret
COOKIE_SECRET=your_cookie_secret
OPENAI_API_KEY=your_openai_api_key
OPENAI_ORG_ID=your_openai_organization_id
