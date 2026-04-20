# JWT Authentication System - Spring Boot

## 📌 Overview

This project is a **secure backend authentication system** built using Spring Boot and Spring Security. It implements **JWT (JSON Web Token) based authentication and authorization** with a layered architecture.

---

## 🚀 Tech Stack

* Java 17+
* Spring Boot
* Spring Security
* JWT (JSON Web Tokens)
* Spring Data JPA
* Hibernate
* H2 / MySQL (configurable)
* Maven

---

## 🔐 Features

* User Registration & Login
* JWT-based Authentication
* Stateless Session Management
* Secure API Endpoints
* Layered Architecture (Controller → Service → Repository)
* DTO-based request/response handling

---

## ⚙️ Project Structure

```
config/      → Security & app configuration  
controller/  → REST API endpoints  
dto/         → Data Transfer Objects  
entity/      → Database models  
repository/  → JPA repositories  
security/    → JWT & authentication logic  
service/     → Business logic  
util/        → Helper utilities  
```

---

## ▶️ How to Run

### 1. Clone the repository

```bash
git clone https://github.com/Prateeeeek423/<your-repo-name>.git
cd <your-repo-name>
```

### 2. Run the application

#### Windows

```bash
.\mvnw.cmd spring-boot:run
```

#### Linux/macOS

```bash
./mvnw spring-boot:run
```

---

## 🌐 API Testing

Use Postman or curl to test endpoints.

### Example Endpoints (may vary)

* `POST /auth/register`
* `POST /auth/login`
* Protected APIs require JWT token in header:

```
Authorization: Bearer <token>
```

---

## 🧪 H2 Console (if enabled)

* URL: http://localhost:8080/h2-console
* JDBC: jdbc:h2:mem:testdb
* Username: sa
* Password: (empty)

---

## 🔐 Security Flow

1. User registers
2. User logs in
3. Server generates JWT token
4. Client sends token in Authorization header
5. Server validates token for protected endpoints

---

## 📈 Future Improvements

* Role-based access control (RBAC)
* Refresh tokens
* Password hashing improvements (BCrypt tuning)
* MySQL/PostgreSQL integration
* Swagger API documentation

---

## 👤 Author

Prateek Yadav
