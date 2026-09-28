# 🚗 CPL — Car Parts, Location & Careers Portal

**CPL** is a centralized automotive platform connecting major car manufacturers (Tata, BMW, Suzuki, Tesla, Mahindra, Hyundai, Toyota, Mercedes-Benz, Audi) with parts buyers and engineering job seekers.

---

## ✨ Features

### 🔧 Spare Parts Catalog (Client / Buyer Mode)
- Browse **EV ⚡ and Fuel ⛽** spare parts from all major auto brands
- Filter by **Brand, Vehicle Type (EV/ICE/Hybrid), Category, Price Range**
- Real-time **stock availability** per dealership location
- Detailed part specs modal with OEM number, rating, and branch-level inventory
- Add parts to **Inquiry Cart** and place stock reservation orders
- **❤️ Favorites & Wishlist System**: 1-click save on any part card or spec modal with localStorage persistence and slide-over wishlist drawer

### 📍 Smart Cities & District-Wise Dealer Locator
- **Smart Cities Search & Filter**: Search all designated Smart Cities (**Pune, Indore, Surat, Ahmedabad, Bengaluru, New Delhi NDMC, Chennai, Hyderabad, Jaipur, Bhopal, Bhubaneswar, Kochi, Lucknow, Chandigarh, Visakhapatnam, Kolkata, Nagpur**)
- **EV Fast Charging Infrastructure**: Shows live count of EV Fast Charging stations at every Smart City hub
- **Smart City Autocomplete in Search Bar**: Instant suggestions with Smart City rank (e.g. *Rank #1 Cleanest Smart City - Indore*, *Rank #1 Smart City Pioneer - Bhubaneswar*)
- **District-Specific Authorized Car Company Networks** (Tata, BMW, Suzuki, Tesla, Mahindra, Hyundai, Toyota, Mercedes, Audi)
- Direct **click-to-call** phone lines and toll-free helplines for every company and branch

### ⛽ Nearest Petrol Pump & CNG Stations (Inside Search Bar)
- **Embedded Search Bar Button**: 1-click access to **"Petrol/CNG"** filling station finder right inside top & hero search bars
- **Live Fuel Prices & CNG Queue Status**: Real-time Petrol, Diesel, and CNG rates with live pump wait times (e.g. *Clear Instant / 2-4 mins*)
- **Authorized Multi-Fuel Networks**: IndianOil (IOCL), Bharat Petroleum (BPCL), HPCL, Shell, Mahanagar Gas (MGL), Indraprastha Gas (IGL), Adani Total Gas, and Jio-bp
- **1-Click Call Pump & Google Maps Navigation**: Direct calling and GPS directions for emergency refueling and CNG filling

### 💼 Engineering Job Portal (Job Seeker Mode)
- Search **Electrical, Mechanical, Embedded, and EV Powertrain** engineering jobs
- Filter by **department, company, and keyword**
- Apply directly with **full candidate profile** (name, email, specialization, experience, cover letter)
- Application submitted to company HR for review

### 🏢 HR Admin Dashboard (Company Mode)
- **Upload new spare parts** to the live website with price, stock count, branch, and vehicle type
- **Post new engineering job openings** for Electrical & Mechanical roles
- **Review candidate applications** — Accept / Shortlist or Reject with status tracking
- Filter applications by company and status

### 👤 Client Registration & Auth
- Register as **Client / Buyer**, **Engineer (Job Seeker)**, or **Company HR Admin**
- Login / Sign-in modal with role and city selection

---

## 🛠️ Tech Stack

| Layer         | Technology                          |
|---------------|-------------------------------------|
| Frontend      | React 19 + Vite 8                   |
| Styling       | Tailwind CSS 4 + Custom CSS tokens  |
| Icons         | Lucide React                        |
| State         | React useState + localStorage       |
| Design System | Glassmorphism, dark mode, neon badges, micro-animations |

---

## 🚀 Getting Started & Run Commands

### 📋 Prerequisites
- **Node.js** v18.0.0 or higher
- **npm** v9.0.0 or higher

### ⚙️ All Terminal Run Commands

| Purpose | Command | Description |
|---|---|---|
| **Install Dependencies** | `npm install` | Installs all React, Vite, Tailwind CSS, Lucide icons & packages |
| **Start Development Server** | `npm run dev` | Starts live HMR dev server at `http://localhost:5173/` |
| **Production Build** | `npm run build` | Compiles optimized production bundle in `/dist` |
| **Preview Production Build** | `npm run preview` | Spins up local server to test the production bundle |
| **Lint & Type Check** | `npm run build -- --logLevel info` | Validates bundle modules and catches syntax errors |

### Quick Start (PowerShell / Terminal)

```powershell
# 1. Navigate to project root
cd "d:\Hey 100rbh\Project\CPL"

# 2. Install dependencies (if first time)
npm install

# 3. Launch live development server
npm run dev


npm  run build
npm run preview

# 4. Open in browser
# http://localhost:5173/
```

---

## 📁 Project Structure

```
CPL/
├── public/
│   └── images/                  # Hero banner, EV battery, engine images
├── src/
│   ├── components/
│   │   ├── Navbar.jsx           # Top navigation, smart search, fuel quick button & role switcher
│   │   ├── HeroBanner.jsx       # Hero section with brand grid, EV filters & petrol/CNG button
│   │   ├── PartsCatalog.jsx     # Filterable parts grid with sidebar filters & wishlist hearts
│   │   ├── PartDetailModal.jsx  # Full specs modal with branch stock breakdown & call action
│   │   ├── DealerLocator.jsx    # Dealer hub cards with per-district stock & EV fast charger stats
│   │   ├── FuelStationModal.jsx # 24/7 Nearest Petrol Pump, CNG & EV Multi-Fuel Station Finder
│   │   ├── FavoritesDrawer.jsx  # Slide-over saved parts wishlist with 1-click cart transfer
│   │   ├── JobPortal.jsx        # Engineering job listings & application form
│   │   ├── HRDashboard.jsx      # HR admin: upload parts, post jobs, review candidate apps
│   │   ├── CartDrawer.jsx       # Slide-over cart with GST pricing, branch pickup & checkout
│   │   └── AuthModal.jsx        # Register / Login modal for Buyer, Engineer & HR roles
│   ├── data/
│   │   └── mockData.js          # Seed dataset: companies, parts, branches, jobs & fuel stations
│   ├── App.jsx                  # Main app with tab routing, modals & localStorage sync
│   ├── main.jsx                 # React 19 entry point
│   └── index.css                # Global styles, glassmorphism, custom design tokens
├── index.html                   # HTML5 template
├── vite.config.js               # Vite 8 build configuration
├── package.json                 # Project dependencies & scripts
└── README.md                    # Comprehensive documentation
```

---

## 🏭 Supported Auto Brands

| Brand            | Type              |
|------------------|-------------------|
| Tata Motors      | EV & Fuel         |
| BMW Group        | Luxury & EV       |
| Maruti Suzuki    | Fuel & Hybrid     |
| Tesla Motors     | Pure EV           |
| Mahindra Auto    | SUV & EV          |
| Hyundai Motor    | EV & Fuel         |
| Toyota Kirloskar | Hybrid & Fuel     |
| Mercedes-Benz    | Luxury & EV       |
| Audi AG          | Performance & EV  |

---

## 📄 License

© 2026 CPL (Car Parts & Location Portal). All rights reserved.
"# CPL" 
