# DataBridge

> Unified data integration & impact reporting for NGOs

## 🎯 Mission

DataBridge empowers NGOs to break down data silos, automate tedious reporting,
and transform fragmented numbers into compelling impact narratives.

## ✨ Features

- **Connect** — No-code connectors for Google Sheets, Excel, CRMs, and more
- **Visualize** — Real-time dashboards showing program outcomes and finances
- **Report** — Automated report generation for funders (USAID, EU, UN, etc.)
- **Narrate** — Impact story builder combining quantitative data with narratives

## 🏗️ Tech Stack

### Backend
- Node.js 20+ with Express.js
- TypeScript (strict mode)
- Prisma ORM with PostgreSQL
- Zod for validation
- JWT for authentication

### Frontend
- React 19 with TypeScript
- Vite for bundling
- TanStack Query for server state
- Tailwind CSS for styling
- shadcn/ui for components

### Infrastructure
- GitHub Actions for CI/CD
- Docker for containerization
- PostgreSQL for database

## 🚀 Quick Start

### Prerequisites
- Node.js 20+
- PostgreSQL 16+
- Git
- Docker (optional)

### Installation

```bash
# Clone the repository
git clone https://github.com/your-username/databridge.git
cd databridge

# Install backend dependencies
cd backend
npm install

# Install frontend dependencies
cd ../frontend
npm install

# Set up environment variables
cp ../.env.example ../.env
# Edit .env with your database credentials

# Set up the database
cd ../backend
npx prisma migrate dev --name init

# Start the backend
npm run dev

# Start the frontend (in a new terminal)
cd ../frontend
npm run dev