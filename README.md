# 📚 Quiz Management System

A secure and efficient RESTful web application for managing MCQ-based quizzes. Built using Spring Boot, this application allows users to register, log in, and take quizzes with automatic result evaluation. Designed with maintainability and performance in mind using Java, SQL, Hibernate, and Spring MVC.

---

## 🔧 Tech Stack

- **Language & Framework**: Java, Spring Boot (Spring MVC)
- **Authentication**: OAuth 2.0
- **Database**: SQL
- **ORM**: Hibernate
- **Testing**: JUnit, Postman

---

## ✨ Features

- 🔐 **Secure Authentication**
  - User registration and login with OAuth 2.0
  - Role-based access control

- 📝 **Quiz Management**
  - Add, update, delete, and view quizzes
  - Attempt quizzes and automatically calculate results

- 🛠 **Full CRUD Support**
  - RESTful APIs for managing quizzes and users
  - Structured MVC architecture for scalability and clean code

- 🔍 **Testing & Quality**
  - Unit tests implemented using JUnit
  - Manual and automated API testing using Postman

---

## 📁 Project Structure

quiz-management-system/
├── src/
│ ├── main/
│ │ ├── java/com/quizapp/
│ │ │ ├── controller/
│ │ │ ├── model/
│ │ │ ├── repository/
│ │ │ ├── service/
│ │ │ └── QuizManagementSystemApplication.java
│ └── test/
│ └── java/com/quizapp/
│ └── QuizServiceTests.java
├── application.properties
├── pom.xml
└── README.md


---

## 🚀 Getting Started

### ✅ Prerequisites

- Java 17+
- Maven
- SQL database (e.g., MySQL/PostgreSQL)
- Postman for API testing

### 🛠 Setup Instructions

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/quiz-management-system.git
   cd quiz-management-system

2.Configure your database:
In application.properties, set your database credentials and connection URL.

3.Build and run the application:

mvn clean install
mvn spring-boot:run
4.Access endpoints using Postman or your preferred API client.
🔐 Authentication Flow (OAuth 2.0)
Users register and log in securely via OAuth 2.0.

JWT tokens are used for session management.

Access is restricted based on user roles.

| Method | Endpoint               | Description               |
| ------ | ---------------------- | ------------------------- |
| POST   | `/api/register`        | Register a new user       |
| POST   | `/api/login`           | Log in and get token      |
| GET    | `/api/quizzes`         | Fetch all quizzes         |
| POST   | `/api/quizzes`         | Add new quiz (admin only) |
| PUT    | `/api/quizzes/{id}`    | Update quiz               |
| DELETE | `/api/quizzes/{id}`    | Delete quiz               |
| POST   | `/api/quizzes/attempt` | Attempt quiz & get result |

✅ Testing
JUnit for unit tests of services and logic

Postman collections created to test all endpoints (CRUD + Auth)

✍️ Author
Kishlay Raj
Java Backend Developer | Passionate about Spring Boot and secure applications
📫 LinkedIn | ✉️ kishlayraj@example.com

📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

---

Let me know if you want a Postman collection `.json`, database schema `.sql`, or Swagger integration too!

