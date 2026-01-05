# MERN Blog Application

A full-stack blog application built with MongoDB, Express, React, and Node.js.

## ✨ New Features (Latest Update)

🎉 Four major features have been added:

1. **📝 Blog Post Summaries** - Auto-generated summaries for blog posts displayed in previews
2. **🏆 Author Badges System** - Gamification badges that reward authors for achievements (FIXED: Now awards properly!)
3. **🎯 Milestones System** - Track long-term progress with 20+ milestones
4. **👑 Admin Dashboard** - Complete admin panel to manage users, roles, and view statistics

## Prerequisites

- Node.js (v14 or higher)
- MongoDB (local or Atlas account)
- Cloudinary account (for image uploads)

## Setup Instructions

### 1. Clone the repository

### 2. Backend Setup

```bash
cd backend
npm install
```

### 3. Frontend Setup

```bash
cd ../frontend
npm install
```

Create a `.env` file in the frontend directory:
```
VITE_API_URL=http://localhost:5000/api
```

## Running the Application

### Start Backend Server
```bash
cd backend
npm start
```

Backend will run on `http://localhost:5000`

### Start Frontend Development Server
```bash
cd frontend
npm run dev
```

Frontend will run on `http://localhost:5173`

## Environment Variables Explanation

### Backend (.env)
- `PORT` - Port number for backend server
- `MONGO_URI` - MongoDB connection string
- `SECRET_KEY` - Secret key for JWT token generation
- `CLOUDINARY_CLOUD_NAME` - Your Cloudinary cloud name
- `CLOUDINARY_API_KEY` - Your Cloudinary API key
- `CLOUDINARY_API_SECRET` - Your Cloudinary API secret
- `FRONTEND_URL` - Frontend URL for CORS configuration

### Frontend (.env)
- `VITE_API_URL` - Backend API base URL

## 🎮 Initialize New Features (One-Time)

After starting both servers:

1. Visit `http://localhost:5173/setup`
2. Click "Initialize All" button
3. Wait for success confirmation
4. Navigate to `/dashboard/achievements` to see badges and milestones

## Features

### Core Features
- User authentication (register/login)
- Create, edit, delete blog posts
- Publish/unpublish blogs
- Comment on blogs
- Like blogs and comments
- User profiles with social links
- Image uploads via Cloudinary

### 🆕 New Features
- **Auto-generated blog summaries** - Concise previews on blog cards
- **Author badges system** - 8 achievement badges (First Post, Trending, Top Rated, etc.) ✅ Fixed awarding!
- **Milestones tracking** - 20+ milestones across 5 categories
- **View tracking** - Track total and unique blog views
- **Author statistics** - Automatic tracking of blogs, views, likes, comments
- **Progress visualization** - Progress bars and completion indicators
- **Gamification dashboard** - Unified view of achievements
- **👑 Admin Dashboard** - Complete admin panel with:
  - User management (view all users with statistics)
  - Role management (promote/demote admins)
  - Platform statistics (users, blogs, comments counts)
  - Protected admin routes
  - Admin-only Setup page access

### 🔐 Admin Features
- **Make Admin** - Promote any user to admin role
- **Remove Admin** - Demote admin back to user
- **View All Users** - Complete user list with blog/comment statistics
- **Dashboard Stats** - Real-time platform metrics
- **Protected Routes** - Admin-only access control
- **Easy Setup** - Simple script to make first admin: `node backend/makeAdmin.js your-Saurabhtbj143@gmail.com`

## Tech Stack

**Frontend:**
- React
- Redux Toolkit
- Vite
- Radix UI (Tabs component)
- TailwindCSS
- Lucide React Icons

**Backend:**
- Node.js
- Express
- MongoDB & Mongoose
- JWT Authentication
- Cloudinary (image storage)
- Bcrypt (password hashing)

## 🏆 Badge System

Authors can earn these badges:
- 🏅 **First Post** - Publish first blog
- 🔥 **Trending Author** - Get 100+ views
- 🚀 **Viral Creator** - Get 1000+ views
- ✍️ **Consistent Writer** - 4-week streak
- 📝 **Dedicated Writer** - 12-week streak
- ⭐ **Top Rated** - 50 total likes
- 🌟 **Highly Acclaimed** - 200 total likes
- 🧠 **Expert Contributor** - 10 posts in one category

## 🎯 Milestone Categories

Track progress in:
- 📌 **Blogs Published** (10, 20, 50, 100)
- 👁️ **Total Views** (100, 500, 1K, 10K, 100K)
- 💬 **Comments Received** (10, 50, 100, 500)
- 📅 **Active Time** (1, 3, 6, 12 months)
- 🌍 **Global Reach** (10, 50, 100, 500 unique readers)

