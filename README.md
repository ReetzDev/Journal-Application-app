# Journal App

A simple Java Spring Boot journal application where users can post their journals. The app provides authentication and authorization using Spring Security and stores data in MongoDB Atlas.

## What is Journal App?
The Journal App is a web-based platform that allows users to write, save, and manage personal journal entries securely. Users can create, read, update, and delete their journals while ensuring data security with authentication and authorization mechanisms. The application is built using Java Spring Boot, providing a robust backend and seamless database integration with MongoDB Atlas.

## Features
- User authentication and authorization with Spring Security
- CRUD operations for journal entries
- RESTful API endpoints
- MongoDB Atlas for cloud-based database storage
- Secure JWT-based authentication

## Technologies Used
- Java 8
- Spring Boot
- Spring Security
- Spring Data MongoDB
- MongoDB Atlas
- RESTful API

## Prerequisites
Ensure you have the following installed before running the project:
- Java 8 or higher
- Maven
- MongoDB Atlas account

## Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/journal-app.git
   cd journal-app
   ```

2. Update `application.properties` with your MongoDB Atlas credentials:
   ```properties
   spring.data.mongodb.uri=mongodb+srv://<username>:<password>@cluster.mongodb.net/journalapp
   ```

3. Build and run the application:
   ```sh
   mvn spring-boot:run
   ```

## API Endpoints

| Method | Endpoint           | Description |
|--------|-------------------|-------------|
| POST   | `/api/auth/register` | Register a new user |
| POST   | `/api/auth/login` | Authenticate user and get JWT token |
| GET    | `/api/journals` | Get all journals (requires authentication) |
| POST   | `/api/journals` | Create a new journal (requires authentication) |
| GET    | `/api/journals/{id}` | Get journal by ID (requires authentication) |
| PUT    | `/api/journals/{id}` | Update journal by ID (requires authentication) |
| DELETE | `/api/journals/{id}` | Delete journal by ID (requires authentication) |

## Authentication
- The application uses JWT authentication.
- Register a new user using the `/api/auth/register` endpoint.
- Obtain a JWT token by logging in through `/api/auth/login`.
- Include the token in the `Authorization` header for protected endpoints:
  ```sh
  Authorization: Bearer your_jwt_token
  ```


### Topics
`java` `spring` `spring-boot` `mongodb` `spring-data` `spring-security` `database-management` `java-8` `springframework` `restful-api` `mongodb-atlas` `journalapp` `spring-boot-project` `mongodb-atlas-cloud` `spring-boot-projects`
