# 💬 Real-Time Chat Application

A modern and scalable real-time chat platform powered by **React.js**, **Node.js**, **Socket.IO**, **MongoDB**, and **Supabase**. It supports one-on-one and group conversations, live typing indicators, media sharing, user presence tracking, and Supabase-based authentication.

---

## 🚀 Features

### ✅ Authentication & Authorization
- Secure login/signup using Supabase Auth
- Role-based access control (Admin/User)
- JWT session management

### 💬 Real-Time Messaging
- One-to-one and group messaging
- Socket.IO for real-time communication
- Typing indicators & seen/delivered status

### 📎 Media Sharing
- Upload images, videos, and files via Supabase Storage
- Preview & download shared media
- File type & size validation

### 🔔 Notifications & Presence
- Online/offline user status
- Toast message notifications
- Push notification integration ready (FCM/Web Push)

### 🔐 Security
- HTTPS-only by default
- JWT-based session management
- Rate limiting, sanitization, and input validation

---

## 🛠️ Tech Stack

### Frontend
- React.js (Vite)
- Tailwind CSS
- Redux Toolkit
- React Router
- Socket.IO Client

### Backend
- Node.js + Express
- Socket.IO
- MongoDB + Mongoose
- Supabase (Auth & Storage)
- JWT Authentication

### Deployment
- Frontend: Vercel / Netlify
- Backend: Render / Railway / AWS EC2
- DB: MongoDB Atlas
- Supabase for storage & auth

---

## 📁 Project Structure

### Frontend (`client/`)
    client/
    ├── public/
    ├── src/
    │ ├── assets/
    │ ├── components/
    │ ├── features/
    │ │ ├── auth/
    │ │ ├── chat/
    │ │ ├── rooms/
    │ │ └── notifications/
    │ ├── hooks/
    │ ├── pages/
    │ ├── redux/
    │ ├── router/
    │ ├── services/
    │ ├── utils/
    │ ├── App.jsx
    │ └── main.jsx
    ├── .env
    ├── tailwind.config.js
    └── vite.config.js


### Backend (`server/`)
    server/
    ├── controllers/
    ├── models/
    ├── routes/
    ├── services/
    ├── socket/
    ├── middlewares/
    ├── config/
    ├── uploads/
    ├── .env
    ├── app.js
    ├── server.js
    └── package.json

---

## ⚙️ Setup & Installation

### Prerequisites
- Node.js (v18+)
- MongoDB (local or MongoDB Atlas)
- Supabase account and project


## 🔧 Backend Setup

```bash
cd server
npm install
```

### Create .env in server/:
```bash
PORT=8080
MONGO_URI=mongodb+srv://<user>:<pass>@cluster.mongodb.net/chatapp
JWT_SECRET=your_jwt_secret
SUPABASE_URL=https://xyzcompany.supabase.co
SUPABASE_KEY=your_service_role_key
```


### Run server:
```bash
npm run dev
```


## 💻 Frontend Setup
```bash
cd client
npm install
```

### Create .env in client/:
```bash
VITE_API_URL=http://localhost:8080/api
VITE_SOCKET_URL=http://localhost:8080
VITE_SUPABASE_URL=https://xyzcompany.supabase.co
VITE_SUPABASE_KEY=your_anon_key
```

### Start the app:
```bash
npm run dev
```

## 🔐 Security & Auth
1. Supabase handles OAuth and Email/Password login
2. JWT used for secure backend APIs.
3. Authorization middleware protects chat endpoints

## 📱 Mobile Friendly
1. Fully responsive using Tailwind CSS
2. Optimized UI for desktop, tablets, and mobile

## 🧩 Future Enhancements
1. 📲 React Native mobile app
2. 📞 Video/audio call integration (WebRTC)
3. 🤖 AI chatbot using OpenAI API
4. 📊 Admin dashboard with analytics
5. 🧾 Chat export (PDF/CSV)

## 👨‍💻 Author
Puneet Yadav

GitHub: @puneetyadav09

Email: puneet932004@gmail.com
