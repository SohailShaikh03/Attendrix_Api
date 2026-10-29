# Attendrix API

A RESTful backend application for attendance management, built with Java and Spring Boot.

## Overview

Attendrix API is a backend project focused on managing attendance-related data through REST endpoints. It demonstrates CRUD operations, layered application design, database integration, and API testing.

## Tech Stack

- **Language:** Java
- **Framework:** Spring Boot
- **Database:** MySQL
- **Build Tool:** Maven
- **API Style:** REST
- **API Testing:** Postman
- **Version Control:** Git and GitHub

## Features

- REST endpoints for attendance-related operations
- CRUD operations for supported resources
- Separation of controller, service, and data-access responsibilities
- Relational database integration
- API testing with Postman

> Update this section to list the exact resources and endpoint paths implemented in your current version.

## Project Structure

A typical Spring Boot layout looks like this. Adjust the package names below to match the actual project structure.

```text
Attendrix_Api/
├── src/
│   └── main/
│       ├── java/
│       │   └── .../
│       │       ├── controller/
│       │       ├── service/
│       │       ├── dao/
│       │       └── entity/
│       └── resources/
│           └── application.properties
├── pom.xml
└── README.md
```

## Prerequisites

Install the following before running the application:

- Java JDK (the version configured in `pom.xml`)
- MySQL Server
- Maven, unless using the Maven Wrapper
- Postman (optional, for testing the API)

## Setup and Run

### 1. Clone the repository

Replace `YOUR_USERNAME` with your GitHub username.

```bash
git clone https://github.com/YOUR_USERNAME/Attendrix_Api.git
cd Attendrix_Api
```

### 2. Create the database

Create the database name expected by your application configuration. For example:

```sql
CREATE DATABASE attendrix;
```

If your project uses a different database name, use that name instead.

### 3. Configure database credentials

Open `src/main/resources/application.properties` and configure the JDBC URL, database username, and password for your local MySQL setup.

Example:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/attendrix
spring.datasource.username=${DB_USERNAME}
spring.datasource.password=${DB_PASSWORD}
```

Set `DB_USERNAME` and `DB_PASSWORD` as environment variables before running the application. Adapt the configuration to match the properties already used by the project. Never commit real credentials or secrets to GitHub.

### 4. Run the application

From the project root:

```bash
mvn spring-boot:run
```

If the project includes the Maven Wrapper, you can use:

**Windows**
```bash
mvnw.cmd spring-boot:run
```

**macOS/Linux**
```bash
./mvnw spring-boot:run
```

Alternatively, import the project into Eclipse as an existing Maven project and run its Spring Boot main class.

### 5. Test the API

Open Postman and send requests to the endpoints implemented in the project. Use the actual paths and request bodies defined by the controllers.

Common HTTP methods:

- `GET` — retrieve data
- `POST` — create data
- `PUT` — update data
- `DELETE` — delete data

## What This Project Demonstrates

- Building REST APIs with Spring Boot
- Implementing CRUD workflows
- Organizing code into application layers
- Connecting Java applications to MySQL
- Testing endpoints with Postman
- Managing code with Git and GitHub

## Possible Future Improvements

- Add request validation and consistent error responses
- Add automated tests with JUnit and Mockito
- Document endpoints with Swagger/OpenAPI
- Add authentication and role-based access control

## Author

**Sohail Ismail Shaikh**

- GitHub: https://github.com/SohailShaikh03

---

This project is intended as a learning and portfolio project for Java backend development.
