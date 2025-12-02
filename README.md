# 🎓 College ERP Frontend (React + Vite + TailwindCSS)

A modern, fully responsive **College ERP Frontend** built with **React, Vite, TailwindCSS**, and connected to a REST API backend.  
This UI is designed to be clean, fast, and beautiful — suitable for real college-level ERP production systems.

---

## ✨ Features

### 🔐 Authentication
- Login page with modern gradient UI
- Backend-connected API auth (`POST /auth/login`)
- Easy to integrate JWT / Session-based login

### 📊 Dashboard
- Attendance summary
- Fees due summary
- Active outpass count
- Upcoming tasks/assignments section
- Clean stat cards and glass UI

### 🗓️ Attendance Module
- Subject-wise attendance
- Progress bars with color-coded safety status
- Date filter (As of Date)
- API: `GET /attendance?date=YYYY-MM-DD`

### 💰 Fees & Payments
- All invoices listed
- Payment button (connected to backend)
- Download receipts (PDF)
- API:
  - `GET /fees`
  - `POST /fees/:id/pay`
  - `GET /fees/:id/receipt`

### 🚪 Outpass System
- Apply for outpass with date + reason + paper less like no need to fill in register simple use QR
- Track status (Approved / Pending / Rejected)
- API:
  - `GET /outpass`
  - `POST /outpass`

### 📚 Assignments
- See all assignments
- Upload & submit assignment files (multipart form-data)
- Submission status
- API:
  - `GET /assignments`
  - `POST /assignments/:id/submit`

### 👤 Profile Page
- Student profile details
- Editable fields layout
- API: `GET /profile`

---

## 🛠️ Tech Stack

- **React 18**
- **Vite**
- **TailwindCSS**
- **Axios**
- **React Router**
- **Modern UI components**
- Responsive Layout (Sidebar + Topbar)

---

## 🔌 Backend API Setup

Add your backend URL in `.env` file:

```env
VITE_API_BASE_URL="http://localhost:4000/api"
```

All API calls are handled through:

```
src/api/client.js
```

---

## 📁 Folder Structure

```
src
├── api
│   └── client.js
├── components
│   ├── Layout.jsx
│   ├── Sidebar.jsx
│   ├── Topbar.jsx
│   ├── StatCard.jsx
│   ├── Badge.jsx
│   └── Table.jsx
├── pages
│   ├── Login.jsx
│   ├── Dashboard.jsx
│   ├── Attendance.jsx
│   ├── Fees.jsx
│   ├── Outpass.jsx
│   ├── Assignments.jsx
│   └── Profile.jsx
└── App.jsx
```

---

## 🚀 Running Locally

```bash
npm install
npm run dev
```

Open the app at:

```
http://localhost:5173
```

---

## 📸 Screenshots (Optional)
*(You can add your own screenshots here)*

---

## 📝 License
This project is free to use and customize for college or personal ERP systems.

---

## ❤️ Support
If you like this project, star the repo ⭐ on GitHub!

If you want help integrating the backend, designing more pages, or deploying — just ask!
