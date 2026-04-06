# 🏥 BD_HealthCare_Backend

A robust, production-ready backend API for a comprehensive healthcare management system. Built with modern technologies, this server handles authentication, user management, doctor and patient profiles, and a seamless appointment booking system with role-based access control.

---

## 🚀 Live API

👉 [https://bd-healthcare-backend.onrender.com]

---

## 📁 Repository

👉 [https://github.com/your-username/BD_HealthCare_Backend]
---

## ⚙️ Tech Stack

| Technology | Purpose |
|------------|---------|
| **Node.js** | JavaScript runtime |
| **Express.js** | Web framework |
| **MongoDB** | NoSQL database |
| **Mongoose** | ODM for MongoDB |
| **JWT** | Authentication & Authorization |
| **bcryptjs** | Password hashing |
| **Express Validator** | Input validation |
| **CORS** | Cross-origin resource sharing |
| **Dotenv** | Environment variables |

---

## 📌 Features

### 🔐 Authentication & Authorization
- User Registration & Login
- JWT Token Generation & Verification
- Role-Based Access Control (Admin, Doctor, Patient)
- Password Encryption (bcrypt)

### 👨‍⚕️ Doctor Management
- Add, update, delete doctors (Admin only)
- Search doctors by specialization, name, or location
- View doctor profiles & availability
- Manage doctor schedules

### 🧑‍🤝‍🧑 Patient Management
- Patient registration & profile management
- View medical history
- Update personal information
- Track appointment history

### 📅 Appointment System
- Book appointments with available doctors
- Cancel or reschedule appointments
- View appointment status (Pending, Confirmed, Completed, Cancelled)
- Prevent double-booking (time slot validation)
- Email notifications (optional)

### 🛡️ Security Features
- JWT-based authentication
- Password hashing with bcrypt
- Input sanitization & validation
- Rate limiting to prevent brute force
- Helmet.js for secure HTTP headers
- Protected routes with middleware

### 📊 Additional Features
- Pagination for large data sets
- Filtering & sorting capabilities
- Error handling middleware
- Request logging (Morgan)
- Environment-based configuration

---
