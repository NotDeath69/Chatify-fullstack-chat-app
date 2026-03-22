# 💬 Chatify — Real-Time Full Stack Chat App

A full-stack real-time chat application built with the MERN stack and Socket.io, deployed on Render.

🔗 **Live Demo:** [chatify-fullstack-chat-app.onrender.com](https://chatify-fullstack-chat-app.onrender.com)

---

## ✨ Features

- 🔐 JWT-based authentication (signup, login, logout)
- 💬 Real-time messaging powered by Socket.io
- 🟢 Online user presence indicators
- 🖼️ Profile picture uploads via Cloudinary
- 🍪 Secure HTTP-only cookie sessions
- 🌐 CORS-enabled REST API
- 📱 Responsive UI

---

## 🛠️ Tech Stack

### Frontend
- React (Vite)
- Tailwind CSS / DaisyUI
- Zustand (state management)
- Socket.io Client
- Axios

### Backend
- Node.js + Express
- MongoDB + Mongoose
- Socket.io
- JWT Authentication
- Cloudinary (image uploads)
- bcryptjs
- dotenv / cookie-parser / cors

---

## 📁 Project Structure

```
Chatify-fullstack-chat-app/
├── backend/
│   ├── src/
│   │   ├── controllers/
│   │   ├── middleware/
│   │   ├── models/
│   │   ├── routes/
│   │   ├── lib/
│   │   │   ├── db.js
│   │   │   └── socket.js
│   │   └── index.js
│   └── package.json
├── frontend/
│   ├── src/
│   └── package.json
└── package.json
```

---

## ⚙️ Setup & Installation

### Prerequisites
- Node.js v18+
- MongoDB Atlas account
- Cloudinary account

### 1. Clone the repo

```bash
git clone https://github.com/NotDeath69/Chatify-fullstack-chat-app.git
cd Chatify-fullstack-chat-app
```

### 2. Install dependencies

```bash
# Install root + backend deps
npm install

# Install frontend deps
cd frontend && npm install
```

### 3. Configure environment variables

Create a `.env` file in the `backend/` folder:

```env
PORT=5001
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
NODE_ENV=development
```

### 4. Run the app

```bash
# Run backend (from root)
npm run dev

# Run frontend (in a separate terminal)
cd frontend && npm run dev
```

Frontend runs on `http://localhost:5173`  
Backend runs on `http://localhost:5001`

---

## 🚀 Deployment

This app is deployed on **Render** (backend + static frontend).

To build for production:

```bash
cd frontend && npm run build
```

The backend serves the frontend's `dist/` folder in production mode via Express static serving.

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

> Built with ❤️ by [NotDeath69](https://github.com/NotDeath69)
