# 📝 Task Manager API

A simple and secure Task Manager REST API built with **Spring Boot**. It features **JWT-based authentication** and supports full **CRUD operations** for users and tasks.

## 🔐 Features

### User Management
- ✅ Register new users
- 🔑 Login with JWT authentication
- ✏️ Update user details
- ❌ Delete users

### Task Management
- 🆕 Create tasks
- 📄 View all tasks (per user)
- 🔁 Update tasks
- 🗑️ Delete tasks

## 🛠️ Tech Stack

- Java 17+
- Spring Boot
- Spring Security + JWT
- Spring Data JPA (Hibernate)
- H2 / MySQL
- Maven

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/task-manager-api.git
cd task-manager-api
2. Configure the Application
Update application.properties or application.yml with your DB settings (H2/MySQL)

Optional: Configure JWT secret and expiration settings

3. Run the Application
bash
Copy code
./mvnw spring-boot:run
The server will start at:

arduino
Copy code
http://localhost:8080/
📬 API Endpoints (Sample)
Auth
Method	Endpoint	Description
POST	/api/auth/register	Register a user
POST	/api/auth/login	Login and get JWT

Users
Method	Endpoint	Description
GET	/api/users/{id}	Get user details
PUT	/api/users/{id}	Update user
DELETE	/api/users/{id}	Delete user

Tasks
Method	Endpoint	Description
GET	/api/tasks	Get all user tasks
POST	/api/tasks	Create a new task
PUT	/api/tasks/{id}	Update a task
DELETE	/api/tasks/{id}	Delete a task

Note: All protected routes require a valid JWT token in the Authorization header.

🔒 Authentication
Use the JWT token returned from /api/auth/login in the header for authorized requests:

http
Copy code
Authorization: Bearer <your-token>
✅ Future Improvements
 Add role-based access (admin/user)

 Add pagination & filtering for tasks

 Swagger/OpenAPI integration

 Dockerize the app
