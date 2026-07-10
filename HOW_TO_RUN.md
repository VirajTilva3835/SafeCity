# SafeCity – Setup & Running Guide

Follow these steps to get the production-ready MERN system running on your local machine.

## 📋 Prerequisites
- **Node.js**: v14+ 
- **MongoDB**: Running locally on `mongodb://localhost:27017`
- **Internet**: Required for Leaflet Map tiles.

---

## 🚀 1. Database Setup & Seeding
First, you MUST seed the database with the city infrastructure (Police/Fire/Hospitals).

```bash
# Navigate to the Backend directory and run seed.js
cd Backend
node seed.js
```

---

## 📡 2. Backend Initialization
```bash
cd Backend
npm install
# Start the server (runs on port 5000)
npm start
```

---

## 💻 3. Frontend Initialization
Open a NEW terminal window:
```bash
cd Frontend
npm install
# Start the production-ready Vite dev server
npm run dev
```

---

## 🔐 Credentials (Auto-Generated)

### 👑 Admin
- **Email**: `admin@safe.com`
- **Password**: `admin123`

### 🚓 Police Stations (Rajkot)
- **Email**: `bdivision@safe.com`, `bhaktinagar@safe.com`, etc.
- **Password**: `bdivision123`, `bhaktinagar123`, etc.

### 🚒 Fire Stations
- **Email**: `mochibazar@safe.com`, `nirmala@safe.com`, etc.
- **Password**: `mochibazar123`, `nirmala123`, etc.

--- 

## 🛠️ Environment Variables
Check `/Backend/.env` if you need to change the MongoDB URI or Port.
Default:
```
PORT=5000
MONGODB_URI=mongodb://localhost:27017/safecity_db
```
