# Tech X Sol - Official Digital Platform

A high-performance modern web platform featuring Interactive Developer Tools, 3D Orbital Hero Animation, Clean Architecture backend, and Neon Serverless PostgreSQL database integration.

---

## 🚀 Quick Start (Local Development)

### 1. Install Dependencies
```bash
npm install
```

### 2. Configure Environment Variables
Copy `.env.example` to `.env`:
```bash
cp .env.example .env
```
Inside `.env`, configure your Neon PostgreSQL Database URL:
```env
PORT=5000
DATABASE_URL=postgresql://neondb_owner:YOUR_PASSWORD@ep-cool-fog-123456.us-east-2.aws.neon.tech/neondb?sslmode=require
JWT_SECRET=your_jwt_secret_key
```
*(Note: If you haven't set `DATABASE_URL` yet, the app runs smoothly with local in-memory fallback!)*

### 3. Start Local Server on Port 5000
```bash
npm run dev
```
Open **`http://localhost:5000`** in your browser.

---

## 🌐 Deploy to Vercel (Production)

This project is built with **Clean Architecture** and is 100% ready for Vercel deployment:

1. **Push to GitHub**:
   ```bash
   git init
   git add .
   git commit -m "Initial Tech X Sol release"
   git branch -M main
   git remote add origin YOUR_GITHUB_REPO_URL
   git push -u origin main
   ```
2. **Deploy on Vercel**:
   * Go to [vercel.com](https://vercel.com) and click **"Add New Project"**.
   * Import your GitHub repository.
   * In **Environment Variables**, add:
     * `DATABASE_URL`: Your Neon PostgreSQL Connection String
     * `JWT_SECRET`: Any secure random key
   * Click **Deploy**.
3. Vercel will automatically serve your static frontend and route `/api/*` requests to the Serverless Backend.

---

## 🛠️ Included Tools Suite (`/tools.html`)
1. **Smart Digital & Digit Calculator**: Number frequency analysis, digit-by-digit breakdown, and digital keypad calculator with history.
2. **Semester CGPA & GPA Calculator**: 4.0 university grading scale, course credit hours, quality points, and cumulative CGPA tracker.
3. **Percentage & Marks Calculator**: Exam marks percentage, grade division, progress meter, and ratio calculators.

