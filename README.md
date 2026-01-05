<div align="center">

# 📝 BuildNotes - MERN Blog Application

### *A Modern Full-Stack Blogging Platform*

[![Made with MERN](https://img.shields.io/badge/Made%20with-MERN-61DAFB?style=for-the-badge&logo=react)](https://github.com/yourusername/MERN-Blog)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=for-the-badge)](http://makeapullrequest.com)

<p align="center">
  <strong>A feature-rich blog application built with MongoDB, Express.js, React, and Node.js</strong>
</p>

[Features](#-features) • [Demo](#-demo) • [Installation](#-installation) • [Tech Stack](#-tech-stack) • [Contributing](#-contributing)

---

</div>

## ✨ New Features (Latest Update)

<div align="center">

### 🎉 Four Major Features Added!

</div>

| Feature | Description |
|---------|-------------|
| 📝 **Blog Post Summaries** | Auto-generated summaries for blog posts displayed in previews |
| 🏆 **Author Badges System** | Gamification badges that reward authors for achievements (FIXED: Now awards properly!) |
| 🎯 **Milestones System** | Track long-term progress with 20+ milestones |
| 👑 **Admin Dashboard** | Complete admin panel to manage users, roles, and view statistics |

---

## 📋 Prerequisites

Before you begin, ensure you have the following installed:

- ![Node.js](https://img.shields.io/badge/Node.js-v14+-339933?style=flat-square&logo=nodedotjs) Node.js (v14 or higher)
- ![MongoDB](https://img.shields.io/badge/MongoDB-Database-47A248?style=flat-square&logo=mongodb) MongoDB (local or Atlas account)
- ![Cloudinary](https://img.shields.io/badge/Cloudinary-Account-3448C5?style=flat-square&logo=cloudinary) Cloudinary account (for image uploads)

---

## 🚀 Installation

### 1️⃣ Clone the repository

```bash
git clone https://github.com/yourusername/MERN-Blog.git
cd MERN-Blog
```

### 2️⃣ Backend Setup

```bash
cd backend
npm install
```

**Create a `.env` file in the backend directory:**

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
SECRET_KEY=your_jwt_secret_key
CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret
FRONTEND_URL=http://localhost:5173
```

### 3️⃣ Frontend Setup

```bash
cd ../frontend
npm install
```

**Create a `.env` file in the frontend directory:**

```env
VITE_API_URL=http://localhost:5000/api
```

---

## 🏃 Running the Application

### Start Backend Server
```bash
cd backend
npm start
```
> Backend will run on `http://localhost:5000`

### Start Frontend Development Server
```bash
cd frontend
npm run dev
```
> Frontend will run on `http://localhost:5173`

---

## 🔐 Environment Variables Explanation

<details>
<summary><b>Backend Environment Variables</b></summary>

| Variable | Description |
|----------|-------------|
| `PORT` | Port number for backend server |
| `MONGO_URI` | MongoDB connection string |
| `SECRET_KEY` | Secret key for JWT token generation |
| `CLOUDINARY_CLOUD_NAME` | Your Cloudinary cloud name |
| `CLOUDINARY_API_KEY` | Your Cloudinary API key |
| `CLOUDINARY_API_SECRET` | Your Cloudinary API secret |
| `FRONTEND_URL` | Frontend URL for CORS configuration |

</details>

<details>
<summary><b>Frontend Environment Variables</b></summary>

| Variable | Description |
|----------|-------------|
| `VITE_API_URL` | Backend API base URL |

</details>

---

## 🎮 Initialize New Features (One-Time Setup)

After starting both servers:

1. Visit `http://localhost:5173/setup`
2. Click **"Initialize All"** button
3. Wait for success confirmation ✅
4. Navigate to `/dashboard/achievements` to see badges and milestones

---

## 🎯 Features

### 🌟 Core Features
- ✅ User authentication (register/login)
- ✅ Create, edit, delete blog posts
- ✅ Publish/unpublish blogs
- ✅ Comment on blogs
- ✅ Like blogs and comments
- ✅ User profiles with social links
- ✅ Image uploads via Cloudinary

### 🆕 Advanced Features
- 📝 **Auto-generated blog summaries** - Concise previews on blog cards
- 🏆 **Author badges system** - 8 achievement badges (First Post, Trending, Top Rated, etc.) ✅ Fixed awarding!
- 🎯 **Milestones tracking** - 20+ milestones across 5 categories
- 👁️ **View tracking** - Track total and unique blog views
- 📊 **Author statistics** - Automatic tracking of blogs, views, likes, comments
- 📈 **Progress visualization** - Progress bars and completion indicators
- 🎮 **Gamification dashboard** - Unified view of achievements

### 👑 Admin Features
- 🔧 **Make Admin** - Promote any user to admin role
- ⬇️ **Remove Admin** - Demote admin back to user
- 👥 **View All Users** - Complete user list with blog/comment statistics
- 📊 **Dashboard Stats** - Real-time platform metrics
- 🔒 **Protected Routes** - Admin-only access control
- ⚡ **Easy Setup** - Simple script to make first admin: 
  ```bash
  node backend/makeAdmin.js your-email@gmail.com
  ```

---

## 🛠️ Tech Stack

<div align="center">

### Frontend
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Redux](https://img.shields.io/badge/Redux-593D88?style=for-the-badge&logo=redux&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)

### Backend
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=JSON%20web%20tokens&logoColor=white)

### Tools & Services
![Cloudinary](https://img.shields.io/badge/Cloudinary-3448C5?style=for-the-badge&logo=cloudinary&logoColor=white)
![Bcrypt](https://img.shields.io/badge/Bcrypt-CA4245?style=for-the-badge)

</div>

<details>
<summary><b>📦 Complete Tech Stack</b></summary>

**Frontend:**
- React - UI library
- Redux Toolkit - State management
- Vite - Build tool
- Radix UI - Component library
- TailwindCSS - Styling
- Lucide React Icons - Icons

**Backend:**
- Node.js - Runtime environment
- Express - Web framework
- MongoDB & Mongoose - Database
- JWT Authentication - Security
- Cloudinary - Image storage
- Bcrypt - Password hashing

</details>

---

## 🏆 Badge System

<div align="center">

### Unlock Amazing Achievements! 🎉

</div>

Authors can earn these badges:

| Badge | Name | Requirement |
|-------|------|-------------|
| 🏅 | **First Post** | Publish your first blog |
| 🔥 | **Trending Author** | Get 100+ views |
| 🚀 | **Viral Creator** | Get 1000+ views |
| ✍️ | **Consistent Writer** | Maintain a 4-week streak |
| 📝 | **Dedicated Writer** | Maintain a 12-week streak |
| ⭐ | **Top Rated** | Receive 50 total likes |
| 🌟 | **Highly Acclaimed** | Receive 200 total likes |
| 🧠 | **Expert Contributor** | Publish 10 posts in one category |

---

## 🎯 Milestone Categories

<div align="center">

### Track Your Progress Across Multiple Categories! 📊

</div>

| Category | Milestones |
|----------|-----------|
| 📌 **Blogs Published** | 10, 20, 50, 100 posts |
| 👁️ **Total Views** | 100, 500, 1K, 10K, 100K views |
| 💬 **Comments Received** | 10, 50, 100, 500 comments |
| 📅 **Active Time** | 1, 3, 6, 12 months |
| 🌍 **Global Reach** | 10, 50, 100, 500 unique readers |

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

### How to Contribute

1. **Fork the repository**
   ```bash
   git clone https://github.com/Saurabhtbj1201/BuildNotes.git
   ```

2. **Create your feature branch**
   ```bash
   git checkout -b feature/AmazingFeature
   ```

3. **Commit your changes**
   ```bash
   git commit -m 'Add some AmazingFeature'
   ```

4. **Push to the branch**
   ```bash
   git push origin feature/AmazingFeature
   ```

5. **Open a Pull Request**

---

## 📝 License

This project is open source and available under the **MIT License**.

---

## 👨‍💻 About Me

### Hi! I'm **Saurabh Kumar** 👋

*A passionate developer focused on automation, AI, and building scalable solutions for real-world problems.*

This project represents my commitment to leveraging modern technologies to streamline e-commerce operations and enhance customer experiences.

### 💼 Skills

`Full-Stack Development` • `MERN Stack` • `API Integration` • `Cloud Services` • `UI/UX Design` • `Database Management` • `DevOps` • `AI & Automation`

<div align="center">

### 🔗 Connect With Me

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/saurabhtbj1201)
[![Twitter](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/saurabhtbj1201)
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://instagram.com/saurabhtbj1201)
[![Facebook](https://img.shields.io/badge/Facebook-1877F2?style=for-the-badge&logo=facebook&logoColor=white)](https://facebook.com/saurabh.tbj)
[![Portfolio](https://img.shields.io/badge/Portfolio-FF5722?style=for-the-badge&logo=todoist&logoColor=white)](https://gu-saurabh.site)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://wa.me/9798024301)

---

<p align="center">
  <strong>Made with ❤️ by Saurabh Kumar</strong>
  <br>
  ⭐ Star this repo if you find it helpful!
</p>

</div>

