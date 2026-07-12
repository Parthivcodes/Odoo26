# REDLINE — Fleet Operations Console 🚛⚡

**REDLINE** is a centralized, smart transport operations platform designed to digitize fleet management for logistics companies. It replaces manual spreadsheets with a single system covering the full lifecycle of transport operations.

<img width="1882" height="898" alt="image" src="https://github.com/user-attachments/assets/adb44fee-44a1-421a-b9b9-78fe49ea2565" />
 


## 🚀 Features

- **Interactive Live Tracking:** Real-time truck routing on an interactive Leaflet map, powered by Geoapify Routing API.
- **Vehicle & Driver Management:** Enforce business rules (no double-booked vehicles, valid license checks, cargo capacity enforcement).
- **Trip Lifecycle Engine:** Manage trips from `Draft` to `Dispatched` to `Completed`, with automatic resource locking.
- **Cost Analytics:** Track fuel costs, maintenance expenses, and automatically calculate trip profitability.
- **Role-Based Access Control:** Secure portal with different access levels (Fleet Manager, Driver, Safety Officer, Financial Analyst).

## 🛠️ Technology Stack

**Frontend** (Next.js)
- Next.js 14 (App Router)
- React 18 & TypeScript
- Tailwind CSS & Framer Motion (Animations)
- Leaflet & React-Leaflet (Interactive Maps)
- Geoapify API (Geocoding & Routing)

**Backend** (Laravel)
- Laravel 11 (PHP 8.2+)
- SQLite / MySQL
- RESTful JSON API

---

## 💻 Getting Started (Local Development)

### 1. Backend Setup (Laravel)
Navigate to the `fleetflow` directory:
```bash
cd fleetflow
composer install
cp .env.example .env
php artisan key:generate
php artisan migrate --seed
php artisan serve
```
*The API will run on http://localhost:8000*

### 2. Frontend Setup (Next.js)
Navigate to the `frontend new/transit-ops-dashboard` directory:
```bash
cd "frontend new/transit-ops-dashboard"
npm install
npm run dev
```
*The web app will run on http://localhost:3000*

## 🗺️ Environment Variables
Make sure you have your Geoapify API key set up in your frontend configuration to enable live map tracking and routing.

## 📄 License
This project was built as a Hackathon Blueprint. All rights reserved.
