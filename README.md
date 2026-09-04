<div align="center">
  <img src="frontend/public/logo.png" alt="ASTRA Logo" width="120" height="120">

  <h1>A S T R A</h1>

  <p>
    <b>ASTRA</b> is your <b>all-in-one competitive programming command center</b> —
    unifying LeetCode, Codeforces, CodeChef, DSA sheets, contests, and analytics into one intelligent dashboard.
  </p>

</div>

---

<h3><b>What is ASTRA?</b></h3>

Tired of juggling five different tabs to track your DSA grind? **ASTRA** brings your entire competitive programming journey — problems, contests, analytics, revision, and progress — into one clean, intelligent ecosystem.

No more manual tracking. No more forgetting which sheet you were on. Just open ASTRA and see everything.

---

<h3><b>Core Features</b></h3>

### 🚀 Unified Dashboard
- All your stats — LeetCode, Codeforces, CodeChef — pulled into a single command center
- Live global rating, total problems solved, and daily streaks at a glance

### 📋 Unified DSA Sheets
- Native tracking for **Striver's A2Z DSA Sheet**, **TLE 31 Sheet (Blind 75)**, and more
- Mark problems solved, flag for revision, and watch your completion bar fill up
- Synced directly from Google Sheets for always up-to-date problem sets

### 📅 Contest Radar
- Every upcoming contest from **Codeforces, LeetCode, CodeChef & AtCoder** — unified into one calendar
- Set reminders, view start times in your local timezone, jump straight to registration

### 📊 Performance Analytics
- Topic-wise radar charts generated from your submission history
- Instantly spot weak spots — Dynamic Programming, Graphs, Trees — and track improvement over time

### 🔁 Intelligent Revision
- Spaced-repetition engine built for competitive programming
- ASTRA auto-flags problems you struggled with and resurfaces them right when you're statistically most likely to forget the approach

### 🎯 Progress Tracking
- Monitor streaks, goals, and daily consistency across every platform

---

<h3><b>Built With</b></h3>

**Frontend**
* [![React][React-badge]][React-url]
* [![Vite][Vite-badge]][Vite-url]
* [![TailwindCSS][Tailwind-badge]][Tailwind-url]
* [![Framer Motion][Framer-badge]][Framer-url]
* Zustand · TanStack Query · Recharts · FullCalendar

**Backend**
* [![NestJS][Nest-badge]][Nest-url]
* [![TypeORM][TypeORM-badge]][TypeORM-url]
* [![PostgreSQL][Postgres-badge]][Postgres-url]
* Passport (JWT · GitHub OAuth · Google OAuth) · Cheerio · Playwright · Puppeteer

---

<h3><b>Project Structure</b></h3>

```sh
ASTRA/
├── backend/                  # NestJS API server
│   └── src/modules/
│       ├── auth/              # JWT + GitHub/Google OAuth
│       ├── leetcode/          # LeetCode scraping & stats
│       ├── codeforces/        # Codeforces scraping & stats
│       ├── codechef/          # CodeChef scraping & stats
│       ├── unified/           # Cross-platform aggregation
│       ├── dashboard/         # Dashboard data
│       ├── sheets/            # A2Z / TLE 31 sheet sync
│       ├── contests/          # Contest calendar
│       ├── analytics/         # Topic-wise performance insights
│       ├── ratings/           # Rating history & graphs
│       ├── progress/          # Streaks & goals
│       ├── submissions/       # Submission history
│       └── profiles / users   # Profile & account management
│
└── frontend/                  # React + Vite client
    └── src/
        ├── pages/              # Dashboard, Sheets, Analytics, Revision, Contest Radar...
        ├── components/         # Cards, charts, tables, sheets UI
        └── api/                # API client layer
```

---

<h3><b>Getting Started</b></h3>

### Prerequisites

* Node.js 18+
* PostgreSQL

### Backend Setup

```sh
cd backend
npm install
cp .env.example .env   # fill in DB, JWT, and Google Sheets API credentials
npm run start:dev
```

### Seed the DSA Sheets

The A2Z and TLE 31 sheet problems need to be seeded into the database before they'll show up in the app:

```sh
cd backend
npm run seed:sheets
```

### Frontend Setup

```sh
cd frontend
npm install
npm run dev
```

---
<p align="center">made with lots of coffee & recursion ☕</p>

[React-badge]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://react.dev/
[Vite-badge]: https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white
[Vite-url]: https://vitejs.dev/
[Tailwind-badge]: https://img.shields.io/badge/TailwindCSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white
[Tailwind-url]: https://tailwindcss.com/
[Framer-badge]: https://img.shields.io/badge/Framer_Motion-black?style=for-the-badge&logo=framer&logoColor=blue
[Framer-url]: https://www.framer.com/motion/
[Nest-badge]: https://img.shields.io/badge/NestJS-E0234E?style=for-the-badge&logo=nestjs&logoColor=white
[Nest-url]: https://nestjs.com/
[TypeORM-badge]: https://img.shields.io/badge/TypeORM-FE0803?style=for-the-badge&logo=typeorm&logoColor=white
[TypeORM-url]: https://typeorm.io/
[Postgres-badge]: https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white
[Postgres-url]: https://www.postgresql.org/
