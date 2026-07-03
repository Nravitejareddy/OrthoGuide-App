# 🦷 OrthoGuide AI
### Intelligent Orthodontic Care & Patient Management Platform

![Android](https://img.shields.io/badge/Android-Kotlin-3DDC84?logo=android)
![Flask](https://img.shields.io/badge/Backend-Flask-000000?logo=flask)
![React](https://img.shields.io/badge/Web-React-61DAFB?logo=react)
![MySQL](https://img.shields.io/badge/Database-MySQL-4479A1?logo=mysql)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

OrthoGuide AI is a full-stack orthodontic healthcare platform designed to streamline communication between patients and clinicians through AI-assisted diagnostics, appointment management, treatment tracking, and secure authentication.

The project consists of a native Android application, a Flask backend, a React web dashboard, and supporting privacy and account management pages.

---

# 📂 Repository Structure

```text
OrthoGuide-App/
│
├── frontend/               # Android Application (Kotlin)
├── backend/                # Flask REST API
├── web/                    # React + Vite Web Dashboard
├── privacy-policy/         # Privacy Policy Website
├── delete-account/         # Google Play Account Deletion Page
│
└── README.md
```

---

# 🏗 System Architecture

```text
                    ┌─────────────────────┐
                    │   React Dashboard   │
                    └──────────┬──────────┘
                               │
                    REST API / JSON
                               │
          ┌────────────────────┼────────────────────┐
          │                    │                    │
          ▼                    ▼                    ▼
    Android App         Flask Backend       AI Assistant
       Kotlin              Python              Ollama
          │                    │
          └──────────────┬─────┘
                         ▼
                   MySQL Database
```

---

# ✨ Key Highlights

- 🤖 AI-powered Orthodontic Assistant with Ollama integration
- 🔐 Secure authentication with OTP verification
- 👨‍⚕️ Clinician and patient management system
- 📅 Appointment scheduling and treatment tracking
- 💬 Intelligent chatbot with FAQ fallback support
- 📊 Interactive clinician dashboard and analytics
- 🔔 Automated reminders and patient notifications
- 📱 Cross-platform ecosystem: Android, Web, and Backend
- ⚡ RESTful API architecture with scalable backend services

---

# 🛠 Technology Stack

| Category | Technologies |
|----------|--------------|
| Mobile | Kotlin, Android Studio, MVVM |
| Backend | Python, Flask, Flask-SQLAlchemy |
| Database | MySQL |
| Authentication | JWT, OTP Verification, Flask-Bcrypt |
| AI | Ollama, FAQ Engine |
| Web | React, Vite, TailwindCSS |
| Networking | Retrofit, OkHttp, Axios |
| Scheduler | APScheduler |
| Deployment Support | Gunicorn |

---

# 📱 Modules

## 📱 Android Mobile Application

> 📖 **Description**  
> Native Android application developed using Kotlin following the MVVM architecture, enabling patients to register, verify OTPs, communicate with the AI assistant, monitor treatment progress, manage appointments, report orthodontic issues, and access essential treatment information directly from their smartphones.

> 🛠 **Tech Stack**  
> Kotlin • Android Studio • MVVM • Retrofit • OkHttp • Gson • ViewBinding • Material Design 3

---

## ⚙ Backend API

> 📖 **Description**  
> Central Flask-based REST API responsible for secure authentication, clinician and patient management, appointment scheduling, AI chatbot integration, OTP verification, automated reminders, notifications, dashboard analytics, and reliable database communication.

> 🛠 **Tech Stack**  
> Python • Flask • Flask-SQLAlchemy • Flask-Bcrypt • Flask-CORS • APScheduler • MySQL • Gunicorn

---

## 🌐 Web Dashboard

> 📖 **Description**  
> Modern and responsive React dashboard designed for clinicians and administrators to manage patients, monitor treatment progress, schedule appointments, visualize analytics, and oversee orthodontic workflows through an intuitive interface.

> 🛠 **Tech Stack**  
> React • Vite • TailwindCSS • Axios • React Router • Framer Motion • Recharts • Radix UI

---

## 🔒 Privacy Policy

> 📖 **Description**  
> Public privacy policy website that explains how user information is collected, processed, stored, and protected, ensuring compliance with Google Play Developer Program requirements.

> 🛠 **Tech Stack**  
> HTML • CSS • JavaScript

---

## 🗑 Account Deletion

> 📖 **Description**  
> Dedicated account deletion portal that enables users to permanently remove their OrthoGuide accounts in accordance with Google Play's User Data and Account Deletion policies.

> 🛠 **Tech Stack**  
> HTML • CSS • JavaScript

---

# 🚀 Getting Started

## 1. Clone Repository

```bash
git clone https://github.com/Nravitejareddy/OrthoGuide-App.git
cd OrthoGuide-App
```

---

## 2. Backend Setup

```bash
cd backend

python -m venv venv

# Windows
venv\Scripts\activate

pip install -r requirements.txt

python app.py
```

**Default Backend URL**

```text
http://localhost:5001
```

---

## 3. Database Setup

Create a MySQL database named:

```text
orthoguide
```

Import the database schema:

```text
orthoguide.sql
```

Update `config.py` with your database credentials.

---

## 4. Web Dashboard Setup

```bash
cd web

npm install

npm run dev
```

Update the API Base URL if required.

---

## 5. Android Application Setup

Open the `frontend` folder using Android Studio.

Update:

```text
RetrofitClient.kt
```

Replace:

```kotlin
private const val BASE_URL = "http://YOUR_LOCAL_IP:5001/"
```

with your local backend address.

Run the application on an emulator or physical Android device.

---

# 📈 Future Roadmap

- 🎥 Integrated Video Consultation
- ☁️ Cloud Deployment and Scalability
- 🔔 Firebase Push Notifications
- 🧠 AI-based Treatment Prediction
- 🦷 Dental Image Analysis
- 🌍 Multi-language Support
- 🔐 Enhanced Role-Based Access Control
- 🏥 Electronic Health Record Integration

---

# 📄 License

This project was developed as an academic project and is maintained for educational and portfolio purposes.

---

# 👨‍💻 Author

**Ravi Teja Reddy N**

Computer Science & Engineering Graduate

🐙 GitHub: <https://github.com/Nravitejareddy>

---

# ⭐ Project Status

> ✅ **Completed** — Core development has been completed successfully and the project is maintained as part of an academic portfolio.

---

> **OrthoGuide AI — Empowering Smiles Through Intelligent Orthodontic Care.**
