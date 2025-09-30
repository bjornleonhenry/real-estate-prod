# Real Estate Management Platform

A comprehensive full-stack real estate management application featuring property listings, tenant management, lease tracking, and application processing.

## Features

- 🏠 Property listing and management
- 👥 Tenant application and management system
- 📋 Lease tracking and document management
- 💳 Payment processing and financial tracking
- 📊 Analytics and reporting dashboard
- 🔐 Role-based access control (managers/tenants)
- 📱 Responsive design for all devices
- 🌐 Multi-location support

## Architecture

This application consists of two main components:

### Frontend (Next.js 14)
- **Tech Stack**: Next.js 14, React, TypeScript, Tailwind CSS, Shadcn/ui
- **Features**: Modern UI, real-time updates, responsive design
- **Location**: `/client` directory

### Backend (Node.js/Express)
- **Tech Stack**: Node.js, Express, TypeScript, Prisma ORM, PostgreSQL
- **Features**: REST API, authentication, database management
- **Location**: `/server` directory

## Getting Started

### Prerequisites

- Node.js (v18 or higher)
- PostgreSQL database
- npm or yarn or pnpm

### Installation

1. **Backend Setup:**
```bash
cd server
npm install
# Set up your database and environment variables
npx prisma migrate dev
npm run dev
```

2. **Frontend Setup:**
```bash
cd client
npm install
npm run dev
```

3. Access the application:
   - Frontend: `http://localhost:3000`
   - Backend API: `http://localhost:8000`

## Environment Variables

### Backend (.env)
```env
DATABASE_URL="your_postgresql_connection_string"
JWT_SECRET="your_jwt_secret"
PORT=8000
```

### Frontend (.env.local)
```env
NEXT_PUBLIC_API_URL=http://localhost:8000
```

## Database Setup

1. Set up your PostgreSQL database
2. Update the `DATABASE_URL` in the server `.env` file
3. Run migrations:
```bash
cd server
npx prisma migrate dev
npx prisma seed  # Optional: seed with sample data
```

## Deployment

### Frontend
Deploy the `/client` directory to Vercel, Netlify, or any modern hosting platform.

### Backend
Deploy the `/server` directory to a VPS, Railway, Render, or similar platform that supports Node.js applications.

## License

MIT License
