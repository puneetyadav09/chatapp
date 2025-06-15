# 💬 Real-Time Chat Application

A secure, scalable real-time chat platform built with **ReactJS**, **Spring Boot**, **WebSocket**, **Redis**, and **JWT** authentication. Supports 1-on-1 and group chats with features like message delivery status, user presence, media sharing, and end-to-end encryption.

---

## 🚀 Features

### ✅ User Authentication & Authorization
- JWT-based login/register
- Role-based access control (Admin/User)
- OAuth (Google/Facebook) ready

### 💬 Real-Time Messaging
- One-to-one direct chat
- Group chat rooms
- Typing indicators & delivery status
- Seen/unseen messages
- STOMP over WebSocket

### 📡 Presence & Notifications
- Online/offline user tracking
- Push notifications (FCM/Web Push)
- Toast notifications

### 📎 Media & File Sharing
- Upload and preview images, videos, docs
- Download shared files
- File size/type validation

### 🔐 Security
- End-to-End Encryption (Signal Protocol integration ready)
- HTTPS only
- Rate limiting & XSS protection
- JWT-based session management

### 🔍 Search & Filters
- Search messages/users
- Filter chats by media/date

---

## 🛠️ Tech Stack

### Frontend
- ReactJS (Vite) + Tailwind CSS
- Redux Toolkit + React Router + Axios
- Socket.IO client
- Progressive Web App (PWA) ready

### Backend
- Java 17 + Spring Boot 3
- Spring Security + JWT + CORS
- WebSocket with STOMP
- Redis Pub/Sub for message broadcasting
- MySQL/PostgreSQL for persistence
- Hibernate/JPA + Lombok

### DevOps & Deployment
- Dockerized backend
- CI/CD via GitHub Actions (optional)
- Frontend: Vercel / Netlify
- Backend: Railway / Render / AWS EC2
- DB: MongoDB Atlas / Supabase / RDS

---

## 🗂 Folder Structure

### Frontend (`client/`)
    client/
    ├── public/
    ├── src/
    │ ├── assets/
    │ ├── components/
    │ ├── features/
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
    ├── src/main/java/com/chatapp/
    │ ├── config/
    │ ├── controller/
    │ ├── dto/
    │ ├── entity/
    │ ├── exception/
    │ ├── repository/
    │ ├── security/
    │ ├── service/
    │ ├── websocket/
    │ └── ChatAppApplication.java
    ├── src/main/resources/
    │ ├── application.properties
    │ └── static/
    ├── src/test/
    ├── Dockerfile
    └── pom.xml



---

## 🧪 Setup & Installation

### Prerequisites
- Java 17+
- Node.js 18+
- Docker (for Redis and backend container)
- MySQL/PostgreSQL instance (local or cloud)

### Backend Setup
```bash
cd server
./mvnw clean install
docker run --name redis -p 6379:6379 -d redis
./mvnw spring-boot:run
```


### Frontend Setup
```bash
cd client
npm install
npm run dev
```


### Environment Variables
client/.env
```bash
VITE_API_URL=http://localhost:8080/api
VITE_SOCKET_URL=http://localhost:8080
```

server/src/main/resources/application.properties
```bash
spring.datasource.url=jdbc:mysql://localhost:3306/chatapp
spring.datasource.username=your_username
spring.datasource.password=your_password
jwt.secret=your_jwt_secret
```


### 🔐 Security & Encryption
This project uses JWT for secure authentication and is structured to integrate Signal Protocol for end-to-end message encryption, ensuring data privacy and integrity between users.


### 📱 Mobile Responsive
The UI is fully responsive, built with Tailwind CSS and designed to work on all screen sizes including tablets and mobile devices.


### 🧩 Future Enhancements
1. 📲 Native mobile app (React Native)

2. 🧠 AI chatbot integration (OpenAI API)

3. 📷 Video/voice call support

4. 🧾 Chat export as PDF

5. 📈 Admin dashboard and analytics


### 👨‍💻 Author
Puneet
GitHub: @puneetyadav09
Email: puneet932004@gmail.com
