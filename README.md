# 🦷 OrthoGuide AI
### Intelligent Orthodontic Care & Patient Management Platform

OrthoGuide AI is a full-stack orthodontic healthcare platform designed to streamline communication between patients and clinicians through AI-assisted diagnostics, appointment management, treatment tracking, and secure authentication.

The project consists of a native Android application, a Flask backend, a React web dashboard, and supporting privacy and account management pages.

---

# 📂 Repository Structure

```
OrthoGuide/
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

```
                    ┌─────────────────────┐
                    │   React Dashboard   │
                    └──────────┬──────────┘
                               │
                    REST API / JSON
                               │
          ┌────────────────────┼────────────────────┐
          │                    │                    │
          ▼                    ▼                    ▼
 Android App            Flask Backend         AI Assistant
   Kotlin                 Python                 Ollama
          │                    │
          └──────────────┬─────┘
                         ▼
                     MySQL Database
```

---

# 📱 Modules

## 📱 Android Mobile Application

Native Android application developed using Kotlin following the MVVM architecture. It enables patients to manage their orthodontic treatment directly from their mobile devices.

### Features

- Patient Login & Registration
- OTP Verification
- AI Chat Assistant
- Treatment Progress Monitoring
- Appointment Tracking
- Incident Reporting
- Offline Data Support
- Material Design UI

### Technology

- Kotlin
- Android Studio
- Retrofit
- OkHttp
- Gson
- ViewBinding
- Material Design 3

---

## ⚙ Backend API

The backend is built using Flask and serves as the central service layer responsible for authentication, AI interactions, patient management, appointments, reminders, and clinician operations.

### Features

- REST API
- JWT Authentication
- OTP Email Verification
- AI Chatbot Integration
- Automated Patient Reminders
- Appointment Management
- Incident Reporting
- Dashboard Analytics

### Technology

- Python
- Flask
- Flask SQLAlchemy
- Flask Bcrypt
- Flask CORS
- APScheduler
- MySQL
- Gunicorn

---

## 🌐 Web Dashboard

Modern responsive dashboard developed using React and Vite for clinicians and administrators.

### Features

- Patient Dashboard
- Clinician Dashboard
- Appointment Management
- Analytics
- Treatment Monitoring
- Responsive Interface

### Technology

- React
- Vite
- TailwindCSS
- Axios
- React Router
- Framer Motion
- Recharts
- Radix UI

---

## 🔒 Privacy Policy

Contains the public Privacy Policy required for deployment on Google Play Store.

---

## 🗑 Account Deletion

Dedicated webpage allowing users to request permanent deletion of their account in accordance with Google Play requirements.

---

# 🤖 AI Features

- AI-powered Orthodontic Assistant
- Intelligent FAQ Engine
- Ollama Local LLM Integration
- Patient Query Resolution
- Treatment Guidance
- Clinical Decision Support

---

# 🔑 Core Features

- AI Assisted Orthodontic Support
- Secure Authentication
- OTP Verification
- Appointment Scheduling
- Treatment Progress Tracking
- Patient Notifications
- Clinician Dashboard
- AI Chatbot
- Incident Reporting
- Automated Reminder System
- Multi-platform Access
- RESTful API Architecture

---

# 🛠 Technology Stack

| Category | Technologies |
|-----------|--------------|
| Mobile | Kotlin, Android Studio |
| Backend | Python, Flask |
| Database | MySQL |
| ORM | Flask SQLAlchemy |
| Authentication | JWT, OTP |
| AI | Ollama |
| Frontend | React, Vite |
| Styling | TailwindCSS |
| Networking | Retrofit, Axios |
| Scheduler | APScheduler |

---

# 🚀 Getting Started

## 1. Clone Repository

```bash
git clone https://github.com/Nravitejareddy/OrthoGuide.git
cd OrthoGuide
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

Backend runs on

```
http://localhost:5001
```

---

## 3. Database Setup

Create a MySQL database named

```
orthoguide
```

Import

```
orthoguide.sql
```

Update

```
config.py
```

with your database credentials.

---

## 4. Web Dashboard

```bash
cd web

npm install

npm run dev
```

Update the API Base URL if required.

---

## 5. Android Application

Open the **frontend** folder using Android Studio.

Update

```
RetrofitClient.kt
```

Replace

```kotlin
private const val BASE_URL = "http://YOUR_LOCAL_IP:5001/"
```

with your local backend address.

Run the application on an emulator or physical Android device.

---

# 📂 Important Directories

```
frontend/
    Android Application

backend/
    Flask REST API

web/
    React Dashboard

privacy-policy/
    Google Play Privacy Policy

delete-account/
    Google Play Account Deletion
```

---

# 📈 Future Improvements

- Video Consultation
- Push Notifications
- Cloud Deployment
- AI Treatment Prediction
- Medical Image Analysis
- Multi-language Support
- Role-based Access Control
- Electronic Health Records Integration

---

# 📄 License

This repository is intended for academic and educational purposes.

---

# 👨‍💻 Author

**Ravi Teja Reddy N**

Computer Science & Engineering

GitHub:
https://github.com/Nravitejareddy

---

# ⭐ Project Status

✅ Active Development

---

> **OrthoGuide AI — Empowering Smiles Through Intelligent Orthodontic Care.**
