# LearnMate
### Agentic AI for Personalized Course Pathways
**IBM AICTE Internship – Problem Statement No. 12**

LearnMate is an **Agentic AI coaching system** that assesses a student's current skill level, understands their learning goals, and generates a personalized, adaptive course roadmap using **IBM Granite** through **IBM watsonx.ai**.

The application consists of a **React frontend** and a **Node.js/Express backend** implementing an agentic perceive–retrieve–decide–act workflow with Retrieval-Augmented Generation (RAG).

---

## Live Demo

**Frontend**
https://learnmate-frontend-delta.vercel.app/

**Backend API**
https://learnmate-backend-1.onrender.com

---

# Repository Structure

```
LearnMate/
│
├── frontend/     # React application
├── backend/      # Node.js + Express API
└── README.md
```

---

# Features

- Personalized course recommendations
- Skill assessment quiz (Beginner / Intermediate / Advanced)
- Multiple learning tracks
- Goal-aware recommendations
- Adaptive roadmap generation
- Progress tracking
- Automatic roadmap replanning
- IBM Granite powered guidance
- Retrieval-Augmented Generation (RAG)

---

# How LearnMate Works

## 1. Perceive

The agent collects:

- Selected learning track
- Skill assessment result
- Student's learning goal
- Completed courses

---

## 2. Retrieve (RAG)

The backend searches a structured course knowledge base and filters courses based on prerequisites already completed.

---

## 3. Decide

The recommendation engine analyzes the student's goal.

Example:

- "Placement ready in 3 months"
- "I want to master backend development"

These produce different recommendations.

---

## 4. Act

IBM Granite generates personalized guidance based on the retrieved roadmap.

---

## 5. Adapt

Whenever a student marks a course complete, the complete recommendation pipeline runs again to generate an updated roadmap.

---

# Tech Stack

## Frontend

- React
- Create React App
- IBM Plex Sans
- IBM Plex Mono
- Unbounded

---

## Backend

- Node.js
- Express
- IBM watsonx.ai
- IBM Granite 4
- IBM Cloud Lite
- Retrieval-Augmented Generation (RAG)

---

# Frontend

Located inside:

```
frontend/
```

Features

- Dashboard interface
- Skill assessment quiz
- Goal input
- Personalized roadmap display
- Course completion tracking
- Live communication with backend

Run locally

```
cd frontend
npm install
npm start
```

Create a `.env` file

```
REACT_APP_API_BASE=http://localhost:5050
```

---

# Backend

Located inside

```
backend/
```

REST Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | /api/tracks | List available tracks |
| POST | /api/roadmap | Generate roadmap |
| POST | /api/progress | Update progress & replan |

Run locally

```
cd backend
npm install
npm start
```

Create a `.env`

```
WATSONX_URL=
WATSONX_PROJECT_ID=
WATSONX_API_KEY=
WATSONX_MODEL_ID=ibm/granite-4-h-small
PORT=5050
```

---

# Project Workflow

```
Student
     │
     ▼
Frontend (React)
     │
     ▼
Backend (Express)
     │
     ▼
Retriever (Knowledge Base)
     │
     ▼
Preference Engine
     │
     ▼
IBM Granite (watsonx.ai)
     │
     ▼
Personalized Roadmap
```

---

# Deployment

Frontend

- Vercel

Backend

- Render

---

# Novel Features

- Adaptive AI-generated learning roadmaps
- Real skill assessment before recommendation
- Goal-aware recommendation engine
- Retrieval-Augmented Generation (RAG)
- IBM Granite-powered explanations
- Dynamic roadmap replanning based on progress

---

# Developed for

IBM AICTE Internship

**Problem Statement No. 12**
**Agentic AI for Personalized Course Pathways**
