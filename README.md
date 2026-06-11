# 💬 Chatty – Real-Time Messaging Platform

Chatty is a full-stack real-time messaging application built with React, Node.js, Express, MongoDB, and Socket.IO. The platform enables users to communicate instantly through secure authentication, persistent chat storage, and low-latency real-time messaging.

## 🚀 Live Demo

🔗 **Live Application:** https://chatt-app-production.up.railway.app/

## 📂 GitHub Repository

🔗 **Source Code:** https://github.com/sjss-178/chatt-app

---

## ✨ Features

* Real-time messaging using Socket.IO
* Secure user authentication and authorization with JWT
* Private one-to-one conversations
* Persistent chat history stored in MongoDB Atlas
* Protected API routes and session management
* Online/offline user status tracking
* Responsive user interface built with React
* Profile image upload and storage using Cloudinary
* Cloud deployment using Railway

---

## 🛠️ Tech Stack

### Frontend

* React
* Zustand
* Tailwind CSS
* Axios

### Backend

* Node.js
* Express.js
* Socket.IO
* JWT Authentication
* REST APIs

### Database

* MongoDB Atlas

### Media Storage

* Cloudinary

### Deployment

* Railway

---

## 🏗️ System Architecture

```text
Frontend (React)
        │
        ▼
Backend (Node.js + Express)
        │
 ┌──────┴──────┐
 ▼             ▼
MongoDB     Socket.IO
 Atlas      Real-Time Layer
        │
        ▼
   Cloudinary
```

---

## 📁 Project Structure

```text
chatty/
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── store/
│   │   ├── hooks/
│   │   └── lib/
│   │
│   └── public/
│
├── backend/
│   ├── controllers/
│   ├── middleware/
│   ├── routes/
│   ├── models/
│   ├── lib/
│   ├── socket/
│   └── server.js
│
└── README.md
```

---

## ⚙️ Prerequisites

Before running the application, ensure you have:

* Node.js (v18 or later)
* npm
* MongoDB Atlas Account
* Cloudinary Account

---

## 🔐 Environment Variables

Create a `.env` file inside the backend directory.

```env
PORT=5001

MONGODB_URI=your_mongodb_atlas_connection_string

JWT_SECRET=your_jwt_secret

CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret

NODE_ENV=development
```

---

## 🗄️ MongoDB Atlas Setup

1. Create an account at https://www.mongodb.com/atlas
2. Create a new cluster.
3. Create a database user.
4. Add your IP address to Network Access.
5. Obtain your MongoDB connection string.
6. Update the `.env` file:

```env
MONGODB_URI=your_connection_string
```

---

## ☁️ Cloudinary Setup

1. Create an account at https://cloudinary.com
2. Open the Cloudinary Dashboard.
3. Copy:

   * Cloud Name
   * API Key
   * API Secret
4. Add them to your `.env` file.

```env
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
```

---

## 🚀 Installation

### Clone Repository

```bash
git clone https://github.com/sjss-178/chatt-app.git
cd chatt-app
```

### Backend Setup

```bash
cd backend
npm install
npm run dev
```

### Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

---

## 🌐 Running the Application

### Backend

```bash
cd backend
npm run dev
```

Runs on:

```text
http://localhost:5001
```

### Frontend

```bash
cd frontend
npm run dev
```

Runs on:

```text
http://localhost:5173
```

---

## 🔒 Authentication Flow

1. User registers or logs in.
2. Server validates credentials.
3. JWT token is generated.
4. Protected routes verify token validity.
5. Authenticated users can access chat functionality.

---

## ⚡ Real-Time Messaging Flow

1. User establishes a Socket.IO connection.
2. Server tracks active users.
3. Messages are emitted instantly through WebSockets.
4. Recipient receives messages in real time.
5. Messages are stored in MongoDB for persistence.

---

## 📈 Future Enhancements

* Group Chats
* Read Receipts
* Typing Indicators
* Message Reactions
* Voice Messages
* Video Calling
* Push Notifications
* End-to-End Encryption

---

## 👨‍💻 Author

**Sontineni Jaswanth Siva Sai**

## 🙏 Acknowledgements

This project was built as part of my learning journey by following and extending the excellent tutorial content created by CodeSistency Youtube Channel.

Tutorial Source:
- https://youtu.be/ntKkVrQqBYY?si=TgSlDHeUUrzWhgpX

I further customized, deployed, and experimented with the project to deepen my understanding of real-time applications, authentication, MongoDB Atlas, Cloudinary integration, and Socket.IO.
