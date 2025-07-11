# 🏀 Masters Basketball Academy (MBA) Portal

A comprehensive web application built for the **Masters Basketball Academy** to manage members, events, registrations, photo/video galleries, and more. The portal includes both a **React frontend** and a **Spring Boot backend**, secured with **AWS Cognito authentication**, and designed for responsive access across devices.

---

## 🔗 Live Repositories

- **Frontend (React)**: [https://github.com/bibhu004/mba-portal](https://github.com/bibhu004/mba-portal)
- **Backend (Spring Boot)**: [https://github.com/bibhu004/mba](https://github.com/bibhu004/mba)

---

## 🧩 Features

### 🔐 Authentication & Security
- User authentication handled via **AWS Cognito** integrated with **AWS Amplify**
- Token-based authentication for secure backend communication
- **Role-based access control** implemented for Admin, Users, and other roles

---

### 📅 Event Management
- Admin can create upcoming events with details like **event name**, **category**, **date**, **time**, and **venue**
- Users can register for available events
- Real-time **countdown timer** displays time left for the next event

---

### 👥 User Account & Team Management
- Users can **create and manage teams** for event registrations
- Real-time teammate addition and validation
- Checks for **age limits**, **gender constraints**, and **team size** as per event rules
- **Progress is saved**, allowing users to pause and resume registration anytime
- Reusable team feature: users can reuse previously created teams and edit them before the event deadline

---

### 🧾 Registration & Invoicing
- Registrations are time-bound, and users must complete them within the allowed period
- **PhonePe (Razorpay)** integrated for secure event payments
- Upon successful payment, users receive a **PDF invoice**
- Users get automated **reminders before the event date**

---

### 🛠️ Admin Panel
- View upcoming events and number of registered participants
- Validate payments, team rosters, and player eligibility
- Upload event-related media (file + metadata)
- Dashboard displays categorized statistics of academy members

---

### ⏱️ Scoreboard (Real-time)
- A full-fledged **real-time basketball scoreboard**
- Separate **controller** and **display** components
- Admin can control and update score, timer, and periods in real time
- The display view updates automatically with all essential match details
- Vertically aligned layout for **home team**, **away team**, and **match timer**

---

### 🖼️ Media Gallery
- Separate sections for **photos** and **videos**
- Photos are grouped by event — click on a photo to view all photos of that event
- Videos highlight **basketball matches**, **tournaments**, **achievements**, and **training**

---

### ⛹️ Coaching Section
- Showcases available **training programs** in an interactive card format
- Each card contains an **image**, **training title**, and **short description**

---

### 🧑‍💼 Member Management
- Admins can **add**, **update**, and **delete** member profiles
- Members are categorized into roles:
  - President, Vice President
  - General Secretary, Organization Secretary
  - Joint Secretary, Advisory Committee
  - Founding Members
- Members are displayed with photos and role-specific groupings

---

### 🌐 Responsive UI
- Mobile-first, fully responsive design using **Tailwind CSS**
- Optimized for all devices — desktop, tablet, and mobile
- Separate styles for login, registration, admin panel, and user dashboard


## 🛠️ Tech Stack

### Frontend
- React.js
- Tailwind CSS
- Axios
- AWS Amplify (Cognito auth)

### Backend
- Java 17
- Spring Boot
- Spring Security
- AWS Cognito JWT token verification
- MySQL
- Multipart file handling via `@RequestParam` and `@RequestPart`
- Swagger (OpenAPI 3)


---

## 🔐 API Security

### Token Verification Flow
- React app sends `Authorization: Bearer <token>` in headers
- Spring Boot backend verifies token with AWS Cognito via Cognito JWT parser
- Secured endpoints for uploading media, managing members, and creating events

---

## 🚀 Setup Instructions

### Frontend

```bash
git clone https://github.com/bibhu004/mba-portal
cd mba-portal
npm install
npm start

### Backend Setup (Spring Boot)

```bash
git clone https://github.com/bibhu004/mba
cd mba
./mvnw spring-boot:run

---

Let me know if you'd like to add deployment instructions (e.g., for AWS EC2/S3), a logo/banner, or a short video demo link.
