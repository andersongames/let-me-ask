# 🧠 Let Me Ask

Let Me Ask is a full-stack application developed during the **NLW Agents** event by **Rocketseat**. It integrates voice input, AI transcription, and conversational intelligence to enable real-time contextual Q&A based on audio streams.

## 🎯 Project Overview

This project demonstrates how to combine web technologies with AI models to build a real-time Q&A platform. Users can record audio which is transcribed, contextualized using AI, and used to answer related questions.

### 🧪 Use Case Example

Imagine a teacher giving a live lecture. As the lecture progresses, students can ask questions, and the AI provides relevant answers based on what has been said so far — without the teacher needing to intervene.

## 📁 Repository Structure

```
/let-me-ask
├── server/   # Backend (API, AI integration, database)
└── web/      # Frontend (UI, audio recording, Q&A interface)
```

> ❗ Although both projects are under the same folder, they are not structured as a monorepo. Each project is set up independently with its own dependencies.

---

## 🧰 Key Technologies

### Backend
- Node.js with native TypeScript
- Fastify
- PostgreSQL + pgvector
- Drizzle ORM
- Google Gemini API
- Zod, Biome, Docker

### Frontend
- React with TypeScript
- Vite + Tailwind CSS
- Shadcn/UI + Radix UI + Lucide
- React Router DOM
- React Hook Form + Zod
- TanStack React Query
- Day.js

---

## ⚙️ Running Locally

### ✅ Prerequisites
- Node.js v18+
- Docker + Docker Compose
- npm or yarn

---

### ▶️ Start the Backend

```bash
git clone <repository-url>
cd let-me-ask/server
cp .env.example .env  # Or manually create .env
docker-compose up -d
npm install
npm run db:migrate
npm run dev
```

> Access API at: http://localhost:3333

---

### 💻 Start the Frontend

```bash
cd let-me-ask/web
npm install
npm run dev
```

> Access app at: http://localhost:5173

---

## 🙌 Acknowledgments

Developed during **NLW Agents** by Rocketseat. This project showcases the power of combining audio capture, transcription, and AI-generated insights in real time.