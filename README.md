# TMS - Task Management / Ticket Tracking System

Full-stack MVP for customer complaint tracking, admin assignment, and employee service updates.

## Stack

- Frontend: React + Vite + React Router + Axios
- Backend: Node.js + Express
- Database: MySQL
- Auth: JWT + bcrypt

## Roles

- `admin`: manage users, view all tickets, assign employees, close tickets
- `customer`: raise complaints and track own tickets
- `employee`: view assigned tickets and submit service updates

## Project Structure

```txt
backend/   Node.js REST API
frontend/  React application
db/        MySQL schema and seed users
```

## Quick Start

### 1. Database

Create a MySQL database:

```sql
CREATE DATABASE tms_system;
```

Then run:

```bash
mysql -u root -p tms_system < db/schema.sql
```

### 2. Backend

```bash
cd backend
npm install
cp .env.example .env
npm run dev
```

Backend runs on `http://localhost:5000`.

### 3. Frontend

```bash
cd frontend
npm install
cp .env.example .env
npm run dev
```

Frontend runs on `http://localhost:5173`.

## Demo Login Users

Password for all demo users: `Password@123`

```txt
admin@sess.co.in      admin
employee@sess.co.in   employee
customer@sess.co.in   customer
```

## Core Flow

```txt
Customer creates complaint
        ↓
Admin reviews open ticket
        ↓
Admin assigns employee
        ↓
Employee updates work/service details
        ↓
Admin closes ticket
```

## Notes

This is an MVP foundation. Next improvements can include file uploads, email/WhatsApp notifications, reports, SLA tracking, and production deployment setup.
