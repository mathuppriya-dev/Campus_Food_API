# 🍽️ Campus Food API (MERN Backend)

This project is a **Node.js + Express + MongoDB REST API** for managing a Campus Food Ordering System.
Campus Food API is a RESTful backend system built using Node.js, Express, and MongoDB to manage students, menu items, and food orders, with support for search, pagination, and analytics.

---

## 📌 Project Description

Campus Food API is a RESTful backend system that allows managing students, menu items, and food orders within a campus environment. It also provides features such as search, pagination, and analytics using MongoDB.

---

## ⚙️ Technologies Used

- Node.js
- Express.js
- MongoDB
- Mongoose
- CORS
- dotenv

---

## 📁 Project Structure

```

campus-food-api/
│
├── models/
│   ├── Student.js
│   ├── MenuItem.js
│   └── Order.js
│
├── routes/
│   ├── students.js
│   ├── menuItems.js
│   ├── orders.js
│   └── analytics.js
│
├── .env
├── package.json
└── server.js

````

---

## 🚀 Setup Instructions

### 1. Install dependencies

```bash
npm install
````

### 2. Create `.env` file

```env
PORT=3000
MONGO_URI=mongodb://127.0.0.1:27017/campus_food
```

👉 Using local MongoDB, so no password is required.

---

### 3. Run the server

```bash
npm start
```

Expected output:

```
Connected to MongoDB
Server running on http://localhost:3000
```

---

## 📡 API Endpoints

### 👤 Students

* `POST /students` → Create student
* `GET /students/:id` → Get student by ID

---

### 🍔 Menu Items

* `POST /menu-items` → Create menu item
* `GET /menu-items` → List all items
* `GET /menu-items/search?name=&category=` → Search items

---

### 🧾 Orders

* `POST /orders` → Place order
* `GET /orders` → Get all orders (pagination)
* `GET /orders/:id` → Get order by ID
* `PATCH /orders/:id/status` → Update status
* `DELETE /orders/:id` → Delete order

---

### 📊 Analytics

* `GET /analytics/total-spent/:studentId`
* `GET /analytics/top-menu-items`
* `GET /analytics/top-menu-items?limit=3`
* `GET /analytics/daily-orders`

---

## 🔍 Key Concepts Used

* Mongoose Schemas for data modeling and validation
* References to connect Student and MenuItem in Orders
* populate() to retrieve related data
* Aggregation pipeline for analytics
* Pagination for efficient data handling
* Regex search for flexible filtering

---

## 🧪 Testing

All APIs are tested using Postman:

* Created at least 3 students
* Created at least 5 menu items
* Placed multiple orders
* Verified all endpoints

---

## 👨‍🎓 Author

* Name: Mathuppriya Naguleswaran
* Student ID: IT24102099
* Course: SE2020 – Web and Mobile Technologies
* Institution: SLIIT

---

## ✅ Status

✔ Completed
✔ Fully working backend
✔ Tested successfully

---

```
```
