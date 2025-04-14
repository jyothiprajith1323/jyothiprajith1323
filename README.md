# 📦 Personal Link & Password Manager

This project is a full-stack secure dashboard that allows you to:
- Store and manage your important links
- Securely save passwords (optional, encrypted)
- Login/logout with JWT authentication

---

## 🧱 Tech Stack

| Component   | Tech                   |
|-------------|------------------------|
| Frontend    | React + TailwindCSS    |
| Backend     | Flask (Python)         |
| Database    | SQLite (easy + portable) |
| Auth        | JWT (JSON Web Token)   |
| Deployment  | Vercel (frontend), Render (backend) |

---

## 📁 Project Structure

```
personal-dashboard/
├── client/         # React + TailwindCSS frontend
├── server/         # Flask backend with JWT + SQLite
└── README.md       # You're here :)
```

---

## 🚀 Deployment Guide

### 1. Backend (Flask) on Render

#### ✅ Step-by-step:

1. Go to [https://render.com](https://render.com)
2. Create a free account if you don’t have one
3. Create a new Web Service → Connect your GitHub
4. Choose the repo that contains your `server/` folder
5. Use the following settings:
   - **Build Command**: `pip install -r requirements.txt`
   - **Start Command**: `python app.py`
   - **Environment Variables**:
     - `SECRET_KEY = your-very-secret-key`
6. Click **Deploy**

Once deployed, you’ll get a backend URL like:
```
https://your-flask-app.onrender.com
```
Save this for the frontend!

---

### 2. Frontend (React) on Vercel

#### ✅ Step-by-step:

1. Go to [https://vercel.com](https://vercel.com)
2. Sign in → Click **Add New Project** → Import from GitHub
3. Select the repo containing your `client/` folder
4. During setup:
   - **Framework**: React (auto-detected)
   - **Environment Variable**:
     - `VITE_API_URL=https://your-flask-app.onrender.com`
5. Click **Deploy**

Now your dashboard is live 🎉

---

## 🛠 Local Development

### 1. Backend (Flask)
```bash
cd server
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python app.py
```

### 2. Frontend (React)
```bash
cd client
npm install
npm run dev
```

---

## ✨ Features

- 🔐 JWT Login & Register
- 🧩 Add / Delete links
- 🔒 Optional password storage with encryption
- ⚡ Responsive & minimal UI (Tailwind)

---

## 📌 TODO / Enhancements

- Add edit functionality
- Add link categories/tags
- Export/import link data (JSON)

---

## 🧡 Made with love using Flask & React

