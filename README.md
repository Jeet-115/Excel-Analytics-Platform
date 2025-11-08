# 🧠 Sheet Sense – Excel Analysis Platform  

An **AI-powered Excel Analysis Platform** built with the **MERN stack** that empowers users to upload, visualize, and analyze Excel data effortlessly.  
Sheet Sense automates chart generation, provides AI-driven insights, supports multilingual interactions, and enables natural language conversations with datasets — all within a secure and interactive web platform.

---

## 📖 Table of Contents
- [Overview](#overview)
- [Problem Statement](#problem-statement)
- [Solution](#solution)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [System Architecture](#system-architecture)
- [User & Admin Workflows](#user--admin-workflows)
- [Data Privacy & AI Integration](#data-privacy--ai-integration)
- [Installation & Setup](#installation--setup)
- [Environment Variables](#environment-variables)
- [Usage](#usage)
- [Future Enhancements](#future-enhancements)
- [Contributors](#contributors)
- [License](#license)

---

## 🧩 Overview

**Sheet Sense** is an intelligent, web-based platform designed to simplify Excel data analysis.  
It allows users to upload Excel files, visualize data through 2D/3D charts, and extract AI-generated insights in multiple languages.  

Users can **chat directly with their datasets**, explore trends, detect anomalies, and gain actionable understanding — without needing advanced analytical knowledge.  

It supports **dual storage options** (local or cloud), ensuring both privacy and accessibility.  
Admins can manage users, files, and monitor platform statistics through a dedicated admin dashboard.

---

## ❗ Problem Statement

Traditional Excel and spreadsheet tools, while powerful, often require technical expertise to generate meaningful insights.  
Users face challenges such as:
- Understanding complex datasets  
- Creating appropriate visualizations manually  
- Deriving trends without analytical background  
- Maintaining privacy when using online tools  

These limitations reduce productivity and accessibility for non-technical users.

---

## 💡 Solution — Sheet Sense

**Sheet Sense** bridges this gap by offering an AI-augmented, user-friendly Excel analysis environment.  

It:
- Automates data visualization using intelligent chart recommendations  
- Provides **AI insights** for trends, anomalies, and data summaries  
- Enables **multilingual AI interactions**  
- Offers **local and cloud storage options** for flexible privacy control  
- Includes **role-based dashboards** for users and admins  

---

## ✨ Features

### 👤 User Features
- **Authentication System**
  - Register/Login with role-based redirection (User/Admin)
- **Excel Upload**
  - Upload files and choose between **local** (temporary) or **database** (persistent) analysis
- **Data Analysis**
  - Select X/Y axes, generate 2D or 3D charts (Bar, Pie, Funnel, Surface, etc.)
  - Receive **AI chart recommendations**
- **AI Insights**
  - Auto-detect trends and anomalies  
  - Generate natural language summaries via OpenAI/Gemini  
  - Export insights as TXT/PDF or share via email
- **Chat with File**
  - Ask questions in natural language and receive AI-driven answers based on your Excel data
- **History Management**
  - View, download, or delete uploaded files
- **Multilingual Support**
  - Available in **English, Hindi, French, Spanish, and Dutch**
- **Profile Settings**
  - Update personal info and password securely

### 🧑‍💼 Admin Features
- **Dashboard Overview**
  - Monitor total users, total files, and analytics
- **User Management**
  - Search, filter, edit, or delete users
- **File Management**
  - View and manage uploaded files
- **Admin Settings**
  - Update admin name and password

---

## 🛠 Tech Stack

### Frontend
- **React.js (v19)** – core frontend framework  
- **Redux Toolkit (v2.7.0)** – global state management  
- **TailwindCSS (v4.1.4)** – styling framework  
- **Chart.js**, **Recharts**, **Three.js** – for 2D/3D data visualization  
- **Framer Motion** – animations  
- **React Router DOM** – routing and navigation  
- **i18next** – multilingual translation support  
- **JSZip**, **html2canvas**, **jsPDF**, **FileSaver** – export and download utilities  

### Backend
- **Node.js + Express.js (v5.1.0)** – backend and REST API  
- **MongoDB + Mongoose (v8.14.0)** – database and ODM  
- **JWT Authentication** – secure login sessions  
- **bcrypt.js** – password encryption  
- **Multer** – Excel file upload handling  
- **Nodemailer** – email and sharing functionality  
- **dotenv, cors, crypto-js, uuid** – configuration and encryption utilities  

### AI Integration
- **OpenAI API / Google Gemini API** – AI-driven insights and conversational analytics  

---

## 🧱 System Architecture

```
SheetSense/
├── backend/                # Node.js + Express server
│   ├── config/             # DB, JWT, AI, Email
│   ├── controllers/        # Core logic for users, files, and AI insights
│   ├── middleware/         # Authentication & file upload
│   ├── models/             # Mongoose schemas
│   ├── routes/             # API endpoints
│   └── utils/              # Helpers and utilities
└── client/                 # React frontend
    ├── components/         # Reusable UI elements
    ├── pages/              # User & Admin dashboards
    ├── services/           # API services
    ├── store/              # Redux slices
    ├── hooks/              # Custom hooks
    └── i18n/               # Multilingual configurations
```

---

## 🔄 User & Admin Workflows

### 🧭 User Workflow
1. Login/Register  
2. Upload Excel file → Choose **local** or **cloud** storage  
3. Analyze data → Select X/Y axes & chart type  
4. View AI insights and anomalies  
5. Chat with the dataset for interactive Q&A  
6. Manage history and settings  

### ⚙️ Admin Workflow
1. Login as Admin  
2. View statistics (users, files, charts)  
3. Manage users (search/edit/delete)  
4. Manage uploaded files  
5. Update admin details securely  

---

## 🔐 Data Privacy & AI Integration

Sheet Sense ensures complete user control and transparency:
- **Dual Storage Model:** Choose local browser analysis or cloud storage  
- **End-to-End Encryption:** JWT + crypto-js secure all data  
- **AI Consent:** User confirmation before sending data to AI APIs  
- **Secure Backend Routing:** Sanitized AI payloads via Express  

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the repository
```bash
git clone https://github.com/Jeet-115/sheetsense.git
cd sheetsense
```

### 2️⃣ Install dependencies
**Backend**
```bash
cd backend
npm install
```
**Frontend**
```bash
cd ../client
npm install
```

### 3️⃣ Run the project
**Backend**
```bash
cd backend
npm run dev
```
**Frontend**
```bash
cd client
npm run dev
```

---

## 🔑 Environment Variables

### Backend (`/backend/.env`)
```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret

# OpenAI / Gemini
OPENAI_API_KEY=your_openai_api_key
GEMINI_API_KEY=your_gemini_api_key

# Email
EMAIL_USER=your_email
EMAIL_PASS=your_password

CLIENT_URL=http://localhost:5173

GOOGLE_APPLICATION_CREDENTIALS=
```

### Frontend (`/client/.env`)
```env
VITE_API_BASE_URL=http://localhost:5000
VITE_CLIENT_URL=http://localhost:5173
```

---

## ▶️ Usage

### For Users
- Sign up or log in  
- Upload Excel file and choose storage option  
- Analyze data with AI-assisted visualization  
- Generate 2D/3D charts  
- Get multilingual AI insights  
- Chat directly with your Excel file  
- Manage uploaded file history and profile  

### For Admins
- Log in as admin  
- View statistics (users, files, activity)  
- Manage user and file records  
- Update admin credentials  

---

## 🚀 Future Enhancements
- Voice-based data queries  
- Real-time multi-user collaboration  
- Predictive analytics and forecasting  
- Mobile app integration  
- Advanced encryption and anonymization  

---

## 👨‍💻 Contributors
- **Jeet**  
- **Pratham**  
- **Maanav**  
- **Dev**
- **Preet**

---

## 📜 License
This project is licensed under the **MIT License**.  
You are free to use, modify, and distribute this project with attribution.
```

