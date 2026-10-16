# ⚡ StylePulse - Luxury Salon Management & Booking Platform

A full-stack salon booking, customer rewards, review analysis (NLP), and salon owner management platform.

---

## 🚀 Quick Start with Docker (Recommended)

Zero configuration, containerized setup for all team members. Runs backend API and frontend web client seamlessly without local Node.js or dependency version conflicts.

### Prerequisites
- [Docker Desktop](https://www.docker.com/products/docker-desktop/) installed and running.

### 1. Clone the repository
```bash
git clone https://github.com/4sTr0J/2026-08-06-salon-test-01.git
cd 2026-08-06-salon-test-01
```

### 2. Environment Configuration
Copy the environment template:
```bash
cp .env.example .env
```
*(Fill in any custom API keys such as Gemini API Key if testing AI Chat features).*

### 3. Build and Run Containers
```bash
docker compose up --build
```

- **Frontend Web App**: [http://localhost:3000](http://localhost:3000) (or [http://localhost:3000/login.html](http://localhost:3000/login.html))
- **Backend API Server**: [http://localhost:5001](http://localhost:5001)

To stop the containers:
```bash
docker compose down
```

---

## 🛠️ Local Development (Without Docker)

If you prefer running directly in Node.js:

### 1. Install all dependencies
```bash
npm run install:all
```

### 2. Start all services concurrently
```bash
npm run dev
```

---

## 📦 Architecture & Key Features

- **Frontend**: Responsive HTML5, Vanilla JavaScript, and CSS3 with Glassmorphic Black & Gold luxury aesthetics.
  - **Customer Portal**: Salon explorer, service menu with multi-column layout, Fresha-style date & time slot booking, card payment authorization, rewards points redemption, appointment rescheduling with dynamic fee enforcement.
  - **Salon Owner Portal**: Live service menu editor with categories, booking calendar with real-time late notifications, order completion & estimated revenue tracking.
  - **Admin Portal**: User verification, platform oversight, and cancellation policy controls.
- **Backend**: Node.js & Express.js (Modular micro-architecture).
  - **Database**: Supabase (PostgreSQL) + Local SQLite (Loyalty & Rewards tracking).
  - **AI & NLP**: Custom review sentiment analysis pipeline + Google Gemini AI assistant.
  - **Scheduling**: Node-cron automated appointment reminders & status processors.

---

## 👥 Contributors

This project was built collaboratively. The following team members each developed their own modules which were integrated into this platform:

| Contributor | GitHub | Module |
|---|---|---|
| **Saneth Rasanjana** | [@SanethRasanjana](https://github.com/SanethRasanjana) | [Frontend UI](https://github.com/SanethRasanjana/TCC-FRONTEND) |
| **Aravinda** | [@Aravinda123-arch](https://github.com/Aravinda123-arch) | [AI Agent](https://github.com/Aravinda123-arch/AI-Agent) |
| **Wasugi** | [@wasugj](https://github.com/wasugj) | [Salon Owner Dashboard](https://github.com/wasugj/salon-owner-dashboard-service) |
| **Oshan Martenstyne** | [@oshanmartenstyne](https://github.com/oshanmartenstyne) | [StylePulse Module](https://github.com/oshanmartenstyne/stylepulseosh) |
| **NiAyo10** | [@NiAyo10](https://github.com/NiAyo10) | NLP & Notifications System |

> See [CONTRIBUTORS.md](./CONTRIBUTORS.md) for full details.