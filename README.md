# 🚀 CloudCode — Real-Time Collaborative Cloud IDE

CloudCode is a real-time collaborative code editor that allows multiple users to work on the same code simultaneously from their browsers.

The project uses **React, Monaco Editor, Yjs, Socket.IO, Node.js, Docker, and AWS** to provide a collaborative coding environment that can be deployed as a containerized cloud application.

---

## ✨ Features

- 📝 Browser-based code editor using Monaco Editor
- 👥 Real-time collaborative code editing
- ⚡ Instant synchronization between multiple users
- 🔄 Conflict resolution using Yjs CRDT
- 🟢 Real-time user presence
- 🔌 Socket.IO-based real-time communication
- ⚛️ React + Vite frontend
- 🟢 Node.js + Express backend
- 🐳 Docker containerization
- ☁️ AWS ECR + ECS deployment
- ❤️ Backend health-check endpoint

---

## 🏗️ Architecture

```text
                         CloudCode
                            │
              ┌─────────────┴─────────────┐
              │                           │
        React Frontend              Node.js Backend
              │                           │
       Monaco Code Editor          Express + Socket.IO
              │                           │
             Yjs                    y-socket.io
              │                           │
              └─────────────┬─────────────┘
                            │
                          Docker
                            │
                           AWS
                            │
                         Users