# Task Manager 

A full-stack Task Manager application built with React (frontend) and Node.js + Express (backend).  
Allows users to create, view, complete, and delete tasks.

🔗 Repository: https://github.com/Aditi-Aditi123/Task-Manager

---

## Tech Stack

- **Frontend:** React (Vite)
- **Backend:** Node.js, Express
- **Storage:** In-memory (no database required)

---

## Project Structure

task-manager/
├── backend/
│   ├── routes/
│   │   └── tasks.js       # All API route handlers
│   └── index.js           # Express server entry point
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   │   ├── AddTaskForm.jsx
│   │   │   ├── TaskItem.jsx
│   │   │   └── TaskList.jsx
│   │   ├── App.jsx
│   │   └── main.jsx
│   └── index.html
└── README.md

---

## Setup & Run Instructions

### Prerequisites
- Node.js v18 or above
- npm

---

### 1. Clone the repository

git clone https://github.com/Aditi-Aditi123/Task-Manager.git
cd Task-Manager

---

### 2. Run the Backend

cd backend
npm install
node index.js

Backend runs at: http://localhost:3000

---

### 3. Run the Frontend

Open a new terminal:

cd frontend
npm install
npm run dev

Frontend runs at: http://localhost:5173

---

## API Endpoints

| Method | Endpoint      | Description          |
|--------|---------------|----------------------|
| GET    | /tasks        | Get all tasks        |
| POST   | /tasks        | Create a new task    |
| PATCH  | /tasks/:id    | Toggle task status   |
| DELETE | /tasks/:id    | Delete a task        |

---

## Task Data Model

| Field      | Type    | Description              |
|------------|---------|--------------------------|
| id         | String  | UUID - unique identifier |
| title      | String  | Task title               |
| completed  | Boolean | Completion status        |
| createdAt  | String  | ISO timestamp            |

---

## Assumptions & Trade-offs

- **In-memory storage** was used instead of a database as permitted by the brief.
  Tasks will reset when the server restarts — acceptable for this exercise.
- **No authentication** was added as this is a single-user local application.
- **Minimal styling** was intentional — the focus was on functionality,
  clean structure, and correct API integration over visual design.
- **CORS** is enabled on the backend to allow the frontend dev server to
  communicate without a proxy setup.
- UUID library is used for reliable unique ID generation instead of Math.random().
