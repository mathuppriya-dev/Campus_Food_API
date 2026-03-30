# 🚀 Campus Food Ordering Backend API

A fully functional backend system built using **Node.js, Express.js, and MongoDB**, designed to manage student food ordering, menu items, and analytics in a scalable and modular way.

---

## 📌 Overview

This project demonstrates how a modern backend application works, including **API development, database integration, middleware usage, and modular architecture**.

It simulates a real-world system where students can place food orders, and the system tracks analytics such as top menu items and total spending.

---
## 🧠 Core Focus: server.js Architecture

This project strongly focuses on the design and structure of the `server.js` file, which acts as the backbone of the backend system.

It is responsible for:
- Initializing the Express application
- Configuring middleware (CORS, JSON parsing)
- Connecting to MongoDB using Mongoose
- Attaching modular route handlers
- Starting the server only after a successful database connection

This demonstrates a clear understanding of backend architecture and execution flow in a real-world Node.js application.

## 🛠️ Tech Stack

* **JavaScript** – Core programming language
* **Node.js** – Server runtime environment
* **Express.js** – Web framework for APIs
* **MongoDB** – NoSQL database
* **Mongoose** – ODM for schema & validation

---

## ⚙️ Features

* 👨‍🎓 Student Management (Create & Retrieve)
* 🍔 Menu Management
* 🧾 Order Processing System
* 📊 Analytics (Top items, spending, daily reports)
* 🔄 RESTful API design
* 🧩 Modular backend architecture
* 🌐 CORS-enabled API communication

---

## 📁 Project Structure

```bash
server/
│
├── routes/
│   ├── students.js
│   ├── menuItems.js
│   ├── orders.js
│   └── analytics.js
│
├── models/
├── server.js
└── .env
```

---

## 🚀 Getting Started

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/your-repo-name.git
cd server
```

### 2️⃣ Install Dependencies

```bash
npm install
```

### 3️⃣ Setup Environment Variables

Create a `.env` file:

```env
PORT=3000
MONGO_URI=mongodb://127.0.0.1:27017/campus_food
```

### 4️⃣ Run the Server

```bash
node server.js
```

👉 Server will run on:
`http://localhost:3000`

---

## 🌐 API Endpoints

### 👨‍🎓 Students

* `POST /students` → Create student
* `GET /students/:id` → Get student

### 🍔 Menu Items

* `GET /menu-items` → Get all menu items

### 🧾 Orders

* `POST /orders` → Create order
* `GET /orders` → Get all orders
* `GET /orders/:id` → Get specific order

### 📊 Analytics

* `GET /analytics/top-menu-items`
* `GET /analytics/daily-orders`
* `GET /analytics/total-spent/:studentId`

---

## 🔄 Backend Workflow

1. Client sends request (Postman / Frontend)
2. Express receives request
3. Middleware processes request (CORS, JSON parsing)
4. Route handler executes logic
5. Mongoose interacts with MongoDB
6. Response is returned to client

Client → Express → Middleware → Routes → Mongoose → MongoDB → Response

---

## 🧠 Key Concepts Demonstrated

* Middleware usage (`cors`, `express.json()`)
* REST API architecture
* Modular routing structure
* Environment variable configuration
* Async database operations
* Error handling

---

## 🧪 Testing

You can test all endpoints using:

* Postman
* Thunder Client (VS Code)

---

## 📌 Author

**Mathuppriya Naguleswaran**

---

## ⭐ Final Note

This project showcases a strong understanding of backend development concepts and real-world API design using the MERN stack. It is structured to be scalable, maintainable, and easy to extend.

---
