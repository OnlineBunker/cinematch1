# 🎬 CineMatch – Full Stack Project

**CineMatch** is a full-stack web application built with the MERN stack that allows users to browse, search, and manage movies effortlessly.
It features secure authentication, movie CRUD operations, reviews, and personalized recommendations powered by React, Node.js, and MongoDB.

---

## 🚀 Project Overview

**Tech Stack**

* **Frontend:** React + React Router + Axios + TailwindCSS
* **Backend:** Node.js + Express.js
* **Database:** MongoDB Atlas
* **Authentication:** JWT (JSON Web Token)
* **Password Security:** Bcrypt Hashing

---

## 🌐 Hosted Links

| Component    | Hosting Platform | Live URL                         |
| ------------ | ---------------- | -------------------------------- |
| **Frontend** | Vercel / Netlify | *(To be added after deployment)* |
| **Backend**  | Render / Railway | *(To be added after deployment)* |
| **Database** | MongoDB Atlas    | Connected                        |

---

## 🧩 Folder Structure

```
CineMatch/
├── client/          # React Frontend  
├── server/          # Express Backend  
├── .env             # Environment variables  
├── package.json     # Project configuration  
└── README.md
```

---

## 🔑 Features

* **User Authentication:** Secure JWT-based login and signup
* **Role Management:** Admin and User access control
* **Movie Management (CRUD):** Admins can create, update, and delete movies
* **Search, Filter & Sort:** Browse movies by title, genre, director, or rating
* **User Interaction:** Rate, review, and bookmark movies
* **Responsive UI:** Built with TailwindCSS and React Router
* **Cloud Hosting:** Deployed using Vercel (frontend), Render (backend), and MongoDB Atlas (database)

---

## 🧠 API Endpoints

| Endpoint                | Method | Description                               | Access        |
| ----------------------- | ------ | ----------------------------------------- | ------------- |
| `/api/auth/signup`      | POST   | Register a new user                       | Public        |
| `/api/auth/login`       | POST   | Authenticate and return JWT               | Public        |
| `/api/movies`           | GET    | Get all movies (with filtering & sorting) | Authenticated |
| `/api/movies/:id`       | GET    | Get details of a single movie             | Authenticated |
| `/api/movies`           | POST   | Add a new movie                           | Admin         |
| `/api/movies/:id`       | PUT    | Update movie details                      | Admin         |
| `/api/movies/:id`       | DELETE | Delete a movie                            | Admin         |
| `/api/reviews/:movieId` | POST   | Add or update review for a movie          | Authenticated |

---

## ⚙️ Setup Instructions

**1️⃣ Clone the Repository**

```bash
git clone https://github.com/yourusername/cinematch.git
cd cinematch
```

**2️⃣ Setup Backend**

```bash
cd server
npm install
```

Create a `.env` file inside `server` with:

```
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
```

Run the backend:

```bash
npm run dev
```

**3️⃣ Setup Frontend**

```bash
cd ../client
npm install
```

Create a `.env` file inside `client` with:

```
VITE_API_URL=http://localhost:5000
```

Run the frontend:

```bash
npm run dev
```

---

