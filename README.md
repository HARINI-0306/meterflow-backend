# MeterFlow Backend 🚀

## 📌 Overview

MeterFlow is a simple API usage tracking and billing system built using Spring Boot.
It allows users to generate API keys, track API usage, and calculate billing based on requests.

---

## ⚙️ Tech Stack

* Java
* Spring Boot
* Spring Data JPA
* H2 Database

---

## ✨ Features

* Create User
* Generate API Key
* Track API Usage
* Calculate Billing

---

## 📂 Project Structure

src/
├── main/
│    ├── java/
│    │    └── controller/
│    │    └── service/
│    │    └── model/
│    │    └── repository/
│    └── resources/
│         └── application.properties

---

## 🚀 API Endpoints

### 1️⃣ Create User

POST /api/user

Request Body:
{
"email": "[test@gmail.com](mailto:test@gmail.com)",
"password": "1234"
}

---

### 2️⃣ Generate API Key

POST /api/key/{userId}

---

### 3️⃣ Use API

GET /api/use?key=YOUR_API_KEY&endpoint=test

---

### 4️⃣ Get Billing

GET /api/billing?key=YOUR_API_KEY

---

## 💡 Billing Logic

* First 1000 requests → Free
* After 1000 → ₹0.005 per request

---

## ▶️ How to Run

1. Open project in VS Code
2. Run `MeterflowApplication.java`
3. Server runs at:
   http://localhost:8080

---

## 🧪 Testing

Use tools like Postman or Thunder Client to test APIs.

---

## 📌 Note

This project uses H2 in-memory database for simplicity.

---

## 👩‍💻 Author

Harini P
