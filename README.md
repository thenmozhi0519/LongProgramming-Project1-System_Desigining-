Student Management System (Spring Boot)

This is a REST API-based mini project built using Spring Boot to perform CRUD operations on student data.
The project uses an H2 in-memory database, making it lightweight and easy to run without external setup.

🛠️ Tech Stack

Java
Spring Boot
Spring Data JPA
H2 Database
Maven
Postman

🏗️ Architecture

Follows a layered structure:

Controller → Service → Repository → Database (H2)
Controller → Handles HTTP requests
Service → Contains business logic
Repository → Interacts with database using JPA
H2 Database → Stores data in-memory

⚙️ Features

Create student
Retrieve all students
Update student details
Delete student
Auto-generated ID

🔗 API Endpoints

Method	Endpoint	Description

GET	/api/students	Get all students
POST	/api/students	Create student
PUT	/api/students/{id}	Update student
DELETE	/api/students/{id}	Delete student

🗄️ Database (H2)

In-memory database (no installation required)
Data resets when application restarts

Access H2 Console:

http://localhost:8080/h2-console
▶️ How to Run
Run StudentApplication.java
Server starts at http://localhost:8080
Test APIs using Postman
🧪 Sample Request (POST)
{
  "firstname": "Thenmozhi",
  "lastname": "E",
  "result": "Pass"
}
🎯 Key Learning
Built REST APIs using Spring Boot
Used JPA to interact with database without writing SQL
Understood layered architecture
Tested APIs using Postman
