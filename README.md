# 🏥 BD_HealthCare_Backend

A robust, production-ready backend API for a comprehensive healthcare management system. Built with modern technologies, this server handles authentication, user management, doctor and patient profiles, and a seamless appointment booking system with role-based access control.

---

## 🚀 Live API

👉 [https://bd-healthcare-backend.onrender.com](https://bd-healthcare-backend.onrender.com)

## 📁 Repository

👉 [https://github.com/your-username/BD_HealthCare_Backend](https://github.com/your-username/BD_HealthCare_Backend)

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
- User registration & login
- JWT token generation & verification
- Role-based access control (Admin, Doctor, Patient)
- Password encryption with bcrypt

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
- Rate limiting to prevent brute force attacks
- Helmet.js for secure HTTP headers
- Protected routes with middleware

### 📊 Additional Features
- Pagination for large data sets
- Filtering & sorting capabilities
- Centralized error handling middleware
- Request logging (Morgan)
- Environment-based configuration

---

## 📂 Project Structure

```
BD_HealthCare_Backend/
├── src/
│   ├── config/          # Database & environment configuration
│   ├── controllers/     # Route controllers
│   ├── middlewares/     # Auth, validation, error handling
│   ├── models/          # Mongoose schemas
│   ├── routes/          # API route definitions
│   ├── utils/           # Helper functions
│   └── app.js           # Express app setup
├── .env.example
├── package.json
└── server.js             # Entry point
```

---

## 🔧 Getting Started

### Prerequisites
- Node.js (v18 or higher)
- MongoDB (local or Atlas connection string)

### Installation

```bash
# Clone the repository
git clone https://github.com/your-username/BD_HealthCare_Backend.git
cd BD_HealthCare_Backend

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env
```

### Environment Variables

Create a `.env` file in the root directory with the following:

```env
PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
JWT_EXPIRES_IN=7d
NODE_ENV=development
```

### Run the Server

```bash
# Development mode
npm run dev

# Production mode
npm start
```

---

## 📡 API Endpoints (Overview)

| Method | Endpoint | Access | Description |
|--------|----------|--------|-------------|
| POST | `/api/auth/register` | Public | Register a new user |
| POST | `/api/auth/login` | Public | Login and receive JWT |
| GET | `/api/doctors` | Public | List/search doctors |
| POST | `/api/doctors` | Admin | Add a new doctor |
| PUT | `/api/doctors/:id` | Admin | Update doctor details |
| DELETE | `/api/doctors/:id` | Admin | Remove a doctor |
| GET | `/api/patients/:id` | Patient/Admin | View patient profile |
| POST | `/api/appointments` | Patient | Book an appointment |
| PUT | `/api/appointments/:id` | Patient/Doctor | Update appointment status |
| DELETE | `/api/appointments/:id` | Patient/Admin | Cancel an appointment |

---

## 🧪 Testing

```bash
npm test
```

---

## 🤝 Contributing

Contributions are welcome! Please open an issue first to discuss what you'd like to change, then submit a pull request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a pull request

---

## 📄 License

This project is licensed under the MIT License.

---

## 👤 Author

Built and maintained by **your-username**.
