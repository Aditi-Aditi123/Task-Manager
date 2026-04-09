# Task Manager

A simple full-stack Task Manager app built with React (frontend) and Node.js/Express (backend).

## Setup & Run

### Backend
cd backend
npm install
node index.js

Runs on http://localhost:3000

### Frontend
cd frontend
npm install
npm run dev

Runs on http://localhost:5173

## Assumptions & Trade-offs
- Used in-memory storage (no database) for simplicity as permitted by the brief.
- Tasks reset on server restart — acceptable for this exercise scope.
- No authentication; this is a single-user local app.
- Focused on functionality and clean structure over visual polish.