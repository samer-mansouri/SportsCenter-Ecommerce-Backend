# 🏋️‍♂️ SportsCenter – E-commerce Backend

A complete backend for a sports e-commerce platform built with **Spring Boot 3**, **MySQL**, **Redis**, **JWT Security**, **Stripe payments**, and **Email notifications**.
It powers features such as authentication, product management, shopping cart, orders, payments, and recommendations.

---

## 🚀 Tech Stack

* **Backend:** Spring Boot 3, Java 17
* **Database:** MySQL 8 (JPA/Hibernate)
* **Cache & Sessions:** Redis
* **Security:** Spring Security, JWT
* **Payments:** Stripe API
* **Email:** SMTP (Gmail)
* **Monitoring:** Spring Boot Actuator
* **Build Tool:** Maven

---

## ✨ Features

* 🔐 User authentication & role-based authorization (JWT)
* 🛍 Product catalog with brands, types, and feedback
* 🛒 Shopping cart & order management
* 💳 Secure payments via **Stripe**
* 📧 Email notifications (order confirmations, etc.)
* ⚡️ Redis caching for performance
* 📊 Health & metrics endpoints with Actuator
* 🤖 External recommendation service integration

---

## ⚙️ Requirements

* Java 17
* Maven 3.8+
* MySQL 8
* Redis

---

## 🛠️ Getting Started

1. **Clone the repository**

   ```bash
   git clone https://github.com/your-username/sportscenter-backend.git
   cd sportscenter-backend
   ```

2. **Set up environment variables** (create a `.env` file in the root directory):

   ```bash
   REDIS_PASSWORD=your_redis_password
   EMAIL_PASSWORD=your_gmail_app_password
   STRIPE_SECRET_KEY=your_stripe_secret
   JWT_SECRET=your_jwt_secret
   ```

3. **Run the application**

   ```bash
   mvn clean package
   mvn spring-boot:run
   ```

4. **Access the API**

   * Backend runs at: `http://localhost:8080`
   * Example health check: `http://localhost:8080/actuator/health`

---

## 🔑 Authentication

* `POST /auth/login` → get JWT access token
* Use header:

  ```
  Authorization: Bearer <token>
  ```

---

## 💳 Payments

Integrated with **Stripe** to handle secure payments.
Requires a valid `STRIPE_SECRET_KEY`.

---

## 📧 Email Notifications

Uses Gmail SMTP to send order and account notifications.
Requires a Gmail App Password stored in `EMAIL_PASSWORD`.

---

## 📜 License

This project is open-source and available under the **MIT License**.

---
