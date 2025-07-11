# 🏀 Masters Basketball Academy (MBA) Portal

A comprehensive web application built for the **Masters Basketball Academy** to manage members, events, registrations, photo/video galleries, and more. The portal includes both a **React frontend** and a **Spring Boot backend**, secured with **AWS Cognito authentication**, and designed for responsive access across devices.

---

## 🔗 Live Repositories

- **Frontend (React)**: [https://github.com/bibhu004/mba-portal](https://github.com/bibhu004/mba-portal)
- **Backend (Spring Boot)**: [https://github.com/bibhu004/mba](https://github.com/bibhu004/mba)

---

## 🧩 Features

### 🔐 Authentication & Security
- AWS Amplify integrated with **AWS Cognito** for secure user login and registration
- Token-based authentication for secure communication with backend APIs

### 🧑‍💼 Member Management
- Add, update, and delete member profiles
- Categorized by roles:
  - President, Vice President
  - General Secretary, Organization Secretary
  - Joint Secretary, Advisory Committee
  - Founding Members
- Photo upload support and role-based display

### 📅 Event Management
- Admin can add upcoming events (with event name, category, date, time, place)
- Users can register for events
- Real-time countdown timer for the next upcoming event

### 🖼️ Media Gallery
- **Photo and video gallery** sections
- Photos grouped by events — click on a preview to view all event photos
- Videos display basketball matches, training, and achievements

### 🧾 Registration & Invoicing
- Postpaid OTT-like subscription model implemented during training phase
- Family/individual account support with **PDF invoice generation**
- Integration with **PhonePe payment gateway**

### 🛠️ Admin Panel
- View upcoming events and number of registered participants
- Upload event media (file + metadata)
- Dashboard with categorized member statistics

### ⛹️ Coaching Section
- Displays 4 training cards in a responsive 2x2 or 4x1 grid
- Each card includes image, name, and description of the training

### ⏱️ Scoreboard (React)
- Timer with start/stop/reset
- Automatically moves to the next period after 10 minutes
- Vertical layout for home team, away team, and timer sections

### 🌐 Responsive UI
- Fully responsive across devices using **Tailwind CSS**
- Custom styling for registration, login, validation, and dashboard pages

---

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

## 🗃️ Folder Structure (Frontend)

