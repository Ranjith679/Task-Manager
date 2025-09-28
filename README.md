📝 Task Manager API (Spring Boot)

A simple Task Manager REST API built with Spring Boot that allows users to manage their tasks efficiently. The app includes user authentication using JWT and supports full CRUD operations for both users and tasks.

🔐 Features

User Authentication

Register new users

Login with JWT token

Update and delete user accounts

Task Management

Create, read, update, and delete tasks

Each task is linked to a specific user

🛠️ Tech Stack

Java + Spring Boot

Spring Security + JWT

Spring Data JPA (Hibernate)

H2 / MySQL (based on configuration)

Maven

🚀 Getting Started

Clone the repo:

git clone https://github.com/your-username/task-manager-api.git


Navigate into the project:

cd task-manager-api


Build and run the app:

./mvnw spring-boot:run


Access the API at:

http://localhost:8080/api/

📬 API Endpoints (Sample)

Auth

POST /api/auth/register – Register a new user

POST /api/auth/login – Login and receive JWT token

Users

GET /api/users/{id} – Get user details

PUT /api/users/{id} – Update user

DELETE /api/users/{id} – Delete user

Tasks

GET /api/tasks – Get all tasks for logged-in user

POST /api/tasks – Create new task

PUT /api/tasks/{id} – Update task

DELETE /api/tasks/{id} – Delete task

✅ To Do

 Add role-based access control

 Swagger/OpenAPI documentation

 Frontend integration
