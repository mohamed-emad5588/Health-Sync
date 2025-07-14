# 🩺 Health-Sync API

**Health-Sync** is a full-featured healthcare Web API built with **.NET 8.0**, designed to connect patients and doctors seamlessly. It enables secure authentication, appointment booking, real-time communication, and administrative monitoring.

---

## 🚀 Features

- 👨‍⚕️ Doctor & Patient management  
- 🔐 Secure authentication using **JWT** with role-based access (Admin, Doctor, Patient)  
- 📅 Appointment booking system  
- 🌟 Doctor ratings and reviews  
- 💬 Real-time chat between patients and doctors using **SignalR**  
- 📧 Email sending via **Gmail SMTP (MailKit)**  
- 🔎 Search functionality (by doctor name, department, etc.)  
- 📊 Admin dashboard endpoints (total users, earnings, appointment stats)

---

## 🛠️ Technologies & Tools

- **.NET 8 / ASP.NET Core Web API**
- **Entity Framework Core**
- **SQL Server**
- **SignalR**
- **JWT Authentication**
- **Gmail SMTP (MailKit)**
- **Swagger / Postman**
- **Git & GitHub**

---

## 📁 Project Structure

```
/Controllers        → API Endpoints (Auth, Doctors, Appointments, Admin, Chat)
/Models             → Domain Entities
/DTOs               → Data Transfer Objects
/Data               → DbContext, Migrations
/Helpers            → Utility classes (e.g. code generators, email formatting, password hashing
/Hubs               → Real-Time Chat Hub
```

---

## 🧪 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/mohamed-emad5588/health-sync.git
```

### 2. Configure the database

Update your `appsettings.json` with your SQL Server connection string.

### 3. Apply migrations

```bash
dotnet ef database update
```

### 4. Run the API

```bash
dotnet run
```

### 5. Access Swagger UI

```
https://localhost:{port}/swagger
```

---

## 🔐 Authentication Flow

- User registration and login
- JWT token returned upon login
- Token used in Authorization header (`Bearer <token>`) to access protected endpoints

---

## 💬 Real-Time Chat with SignalR

- SignalR hub enables live chat between doctors and patients
- Each user joins a group via their ID
- Messages are sent and received instantly

---

## 📧 Email Integration

- Integrated with Gmail SMTP using **MailKit**
- Used for:
  - Account confirmation
  - Booking notifications
  - Admin alerts

---

## 📊 Admin Dashboard APIs

- Total users by role (Admin, Doctor, Patient)
- Total number of appointments
- Total earnings per doctor
- Most active doctors
- Daily/weekly stats (optional)

---

## 👨‍💻 Author

**Mohamed Emad**  
📧 me619251@gmail.com  
🔗 [GitHub Profile](https://github.com/mohamed-emad5588)

---

## 📝 License

This project is licensed under the **MIT License**.
