

---

# 🏥 Cetalink – Smart Healthcare Platform

## 🌐 Overview

**Cetalink** is a smart healthcare web platform designed to connect **patients**, **hospitals**, and **medical stores** in one seamless system.
Users can check symptoms, view nearby hospitals and medicals, and get results or recommendations instantly.

The system uses **Node.js**, **Express**, and **MongoDB** for the backend, along with **EJS templating** for dynamic views. It provides a responsive, user-friendly interface that improves healthcare accessibility and simplifies the process of finding hospitals and medical facilities.

🎥 **Project Demo (YouTube):** [https://youtu.be/YOUR_PROJECT_LINK_HERE](https://youtu.be/YOUR_PROJECT_LINK_HERE)

---

## 🧩 Key Features

### 👩‍⚕️ For Users / Patients

* Register or log in to access the platform.
* Enter symptoms and get medical recommendations.
* View nearby hospitals and medical stores.
* Access detailed hospital/medical shop information.

### 🏥 For Hospitals & Medicals

* List services and specialties.
* Update contact information and facility details.
* Help patients find relevant departments faster.

### ⚙️ For Admins (if extended)

* Manage hospitals, medicals, and user information.
* Review usage data and analytics (future scope).

---

## 🏗️ System Architecture

```
 ┌────────────────────────────────────────────┐
 │                FRONTEND                    │
 │   • EJS Templates (views/)                │
 │   • Static CSS, JS, and Images (public/)  │
 │   • Handles forms for login/signup/search │
 └────────────────────────────────────────────┘
                     │
                     ▼
 ┌────────────────────────────────────────────┐
 │                BACKEND                     │
 │   • Node.js + Express.js server (ceta.js)  │
 │   • Routing and middleware handling        │
 │   • Connects to MongoDB using Mongoose     │
 │   • Loads env variables from .env          │
 └────────────────────────────────────────────┘
                     │
                     ▼
 ┌────────────────────────────────────────────┐
 │                DATABASE                    │
 │        MongoDB (User Data, Hospitals, etc.) │
 │   • users collection (from models/user.js)  │
 │   • medical & hospital collections (future) │
 └────────────────────────────────────────────┘
```

---

## 🛠️ Tech Stack

| Layer                      | Technology                         | Description                                          |
| -------------------------- | ---------------------------------- | ---------------------------------------------------- |
| **Backend Framework**      | Node.js + Express.js               | Handles all routing, logic, and server communication |
| **Frontend Engine**        | EJS                                | Dynamic rendering for HTML templates                 |
| **Database**               | MongoDB + Mongoose                 | Stores users, hospitals, and medical data            |
| **Styling**                | CSS                                | Used for UI/UX design in `/public`                   |
| **Environment Management** | dotenv                             | Manages environment variables from `.env`            |
| **Authentication**         | bcrypt / sessions (if implemented) | Secure user authentication and password storage      |
| **Version Control**        | Git                                | For collaborative development                        |

---

## 📁 Project Structure

```
Cetalink-master/
│
├── ceta.js                # Main server file
├── package.json           # Node dependencies
├── .env                   # Environment variables
│
├── models/
│   └── user.js            # Mongoose schema for user details
│
├── views/                 # EJS templates for frontend
│   ├── home.ejs
│   ├── login.ejs
│   ├── signup.ejs
│   ├── hospitals.ejs
│   ├── medicals.ejs
│   ├── questions.ejs
│   ├── results.ejs
│   └── hospital-details.ejs
│
├── public/                # Static assets
│   ├── *.css              # Styling files
│   ├── *.png, *.jpg       # Images
│   └── JS scripts (if any)
│
└── README.md              # Documentation
```

---

## ⚙️ Installation & Setup

### 🔧 Prerequisites

Make sure you have:

* Node.js (v18 or newer)
* MongoDB (installed and running locally or via cloud)

### 🚀 Steps to Run

```bash
# 1. Clone the repository
git clone https://github.com/yourusername/Cetalink.git
cd Cetalink-master

# 2. Install dependencies
npm install

# 3. Create a .env file
touch .env
```

Inside `.env`, add your environment variables:

```
PORT=3000
MONGODB_URI=mongodb://localhost:27017/cetalink
SESSION_SECRET=your_secret_key
```

```bash
# 4. Start the server
node ceta.js
```

Visit 👉 **[http://localhost:3000](http://localhost:3000)**

---

## 🧠 Application Flow

1. **User lands on homepage (`home.ejs`)** → brief introduction to platform.
2. **Signup/Login** → user credentials stored in MongoDB (`user.js` schema).
3. **Symptom Checker / Questionnaire** (`questions.ejs`) → user enters symptoms.
4. **Result Page (`results.ejs`)** → displays probable issues or suggestions.
5. **Hospital/Medical Finder** (`hospitals.ejs`, `medicals.ejs`) → shows nearby healthcare options.
6. **Details Pages** (`hospital-details.ejs`, `medical-shop-details.ejs`) → shows contact, location, etc.
7. **Logout or Revisit** → ends session securely.

---

## 🧾 Features in Development / Future Scope

* 🩺 AI-based symptom diagnosis system.
* 📍 Google Maps integration for location-based hospital search.
* 📊 Admin dashboard for analytics and data visualization.
* 📱 Responsive mobile-first redesign.
* 🔔 Notification and appointment booking module.

---

## 🤝 Contribution

Want to improve this project?

1. Fork the repo
2. Create a feature branch (`git checkout -b feature-name`)
3. Commit changes (`git commit -m "Added feature"`)
4. Push to your branch (`git push origin feature-name`)
5. Create a Pull Request

---


## 📽️ Demo

🎬 **Watch the full working demo on YouTube:**
👉 Youtube video : https://youtu.be/sa58KAoIzAw?feature=shared
---

## 🏁 Conclusion

**Cetalink** bridges the gap between users and healthcare facilities using a simple yet powerful web interface.
With scalability, modularity, and real-time database integration, it aims to become a one-stop healthcare accessibility platform.

---




