```Student Management System```

This project demonstrates a simple backend REST API built using Spring Boot to manage student data.
It supports basic CRUD operations and uses an H2 in-memory database for quick setup and testing.

Overview

The application allows users to:

Add new student records
View all students
Update student details
Delete student records

It follows a layered architecture to separate concerns and maintain clean code.

Technologies Used

Java
Spring Boot
Spring Data JPA
H2 Database
Maven
Postman

Project Structure
```
com.example.student
│
├── StudentApplication.java
│
├── DAO
│   └── Students.java
│
├── Service
│   └── StudentService.java
│
├── Controller
│   └── StudentController.java
|
├── Repository
│   └── StudentRepository.java
```
Architecture

The application follows a standard layered architecture:

Client → Controller → Service → Repository → Database (H2)

Controller handles HTTP requests
Service contains business logic
Repository interacts with the database
H2 stores data in memory

API Endpoints

GET	/api/students	Retrieve all students
POST	/api/students	Create a new student
PUT	/api/students/{id}	Update student
DELETE	/api/students/{id}	Delete student

Sample Request

POST /api/students
{
  "firstname": "Thenmozhi",
  "lastname": "E",
  "result": "Pass"
}

Database
The project uses H2 in-memory database:

Key Learnings

Built REST APIs using Spring Boot
Used JPA for database interaction
Understood layered architecture
Performed API testing using Postmansing Postman
