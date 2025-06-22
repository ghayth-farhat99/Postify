# Postify - Social Sharing Platform

A modern social platform built with **Next.js** (frontend) and **NestJS** (backend) for seamless post creation, discussions, and interactions.

## ✨ Features
- 📝 Create and share posts
- 💬 Comment on posts
- ❤️ Like/unlike posts
- 🔐 Google OAuth login
- ⚡ Real-time interactions

## 🛠️ Tech Stack
| Frontend | Backend | Database | Auth |
|----------|---------|----------|------|
| Next.js | NestJS | SQLite | JWT |
| TypeScript | Prisma | GraphQL | Google OAuth |

## 📂 Project Structure
postify/
├── apps/
│   ├── front/      # Next.js (port 3000)
│   └── api/        # NestJS + GraphQL (port 8000)
├── packages/       # Shared configs
├── turbo.json      # Turborepo pipelines
└── package.json    # Root workspace


## 🚀 Quick Start

### 1. Clone & Setup
```bash
git clone https://github.com/ghayth-farhat99/Postify.git
 
cd postify

# Install root dependencies
npm install

# Install frontend dependencies
cd apps/front && npm install

# Install backend dependencies
cd ../api && npm install
```

### 2. Configure Environment
Create .env in /apps/api/:
```bash
# Database
DATABASE_URL="file:./dev.db"

# Auth
JWT_SECRET=your_jwt_secret_here
JWT_EXPIRES_IN=24h

# Google OAuth
GOOGLE_CLIENT_ID=your_client_id
GOOGLE_CLIENT_SECRET=your_client_secret
GOOGLE_CALLBACK_URL=http://localhost:8000/auth/google/callback
```

### 3.Run the App
```bash
npm run dev
```