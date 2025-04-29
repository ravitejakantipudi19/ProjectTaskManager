# 📊 Project Tracker

A full-stack project tracking application built with **React**, **Node.js**, **Express**, and **MongoDB**. It allows users to register, log in, and manage projects with authentication and secure backend integration.

---

## 🔧 Technologies Used

### Frontend:
- React
- React Router
- Context API
- Axios
- CSS

### Backend:
- Node.js
- Express
- MongoDB
- Mongoose
- JWT (JSON Web Tokens)
- bcryptjs (Password hashing)

---

## 📁 Project Structure

```
tracker/
│
├── backend/                 # Backend server
│   ├── .env                 # Environment variables
│   ├── package.json         # Backend dependencies
│   └── src/
│       ├── app.js           # Express app setup
│       ├── server.js        # Entry point
│       ├── configs/
│       │   └── db.js        # MongoDB connection
│       ├── controllers/
│       │   └── userController.js  # Handles user routes logic
│       ├── middlewares/
│       │   └── authMiddleware.js  # JWT auth check
│       ├── models/
│       │   ├── userModel.js       # User schema
│       │   └── projectModel.js    # Project schema
│       └── routes/
│           └── index.js           # Route definitions
│
└── frontend/                # React client
    ├── .env                 # API base URL
    ├── package.json         # Frontend dependencies
    ├── public/
    │   ├── index.html       # Main HTML file
    │   └── images, icons    # Logos and assets
    └── src/
        ├── App.js           # Main component and routes
        ├── index.js         # React entry point
        ├── App.css          # Global styles
        ├── components/
        │   ├── Login.js         # Login form
        │   ├── signup.js        # Signup form
        │   ├── Home.js          # Home/dashboard
        │   ├── ProjectView.js   # Display project info
        │   ├── Navbar.js        # Navigation bar
        │   ├── AuthContext.js   # Global auth state
        │   └── ToastContext.js  # Notification context
```

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/your-username/tracker.git
cd tracker
```

---

## ⚙️ Backend Setup

```bash
cd backend
npm install
```

### Create a `.env` file in `backend/` with:

```
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
```

### Start Backend Server

```bash
npm run dev
```

---

## 🌐 Frontend Setup

```bash
cd frontend
npm install
```

### Create a `.env` file in `frontend/` with:

```
REACT_APP_API_URL=http://localhost:5000/api
```

### Start React App

```bash
npm start
```

---

## ✅ Features

- User authentication (signup, login)
- JWT-protected routes
- Project listing & viewing
- Toast notification system
- Global auth state with React Context

---

## 🛡️ Security

- Passwords are hashed using bcryptjs.
- JWT is used for secure token-based authentication.
- Environment variables are used for sensitive configs.

---

## 📝 License

This project is open-source and available under the [MIT License](LICENSE).

---

## 📬 Contact

If you have any questions or suggestions, feel free to contact [your-email@example.com].
