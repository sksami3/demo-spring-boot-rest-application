
# Spring Boot REST API with MySQL

This is a simple RESTful API project built with **Spring Boot**, integrated with **MySQL**, and following a **3-layered architecture**: Controller, Service, and Repository.
```

## Requirements

- **Java 17+**
- **MySQL** 8.x or above
- **Maven** 3.x

## Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/sksami3/demo-spring-boot-rest-application.git
```

### 2. Configure Database
Update the **application.properties** file with your MySQL connection details:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/ems?useSSL=false&allowPublicKeyRetrieval=true
spring.datasource.username=your_mysql_username
spring.datasource.password=your_mysql_password
spring.jpa.hibernate.ddl-auto=update
```

### 3. Build and Run the Application
To build and run the application, use Maven:
```bash
mvn clean install
mvn spring-boot:run
```

## REST API Endpoints

| Method | Endpoint               | Description              |
|--------|------------------------|--------------------------|
| POST   | `/api/employees`        | Create a new employee    |
| GET    | `/api/employees`        | Get all employees        |
| GET    | `/api/employees/{id}`   | Get employee by ID       |
| PUT    | `/api/employees/{id}`   | Update an employee       |
| DELETE | `/api/employees/{id}`   | Delete an employee       |

### Sample JSON for Creating an Employee:
```json
{
  "firstname": "Sheikh",
  "lastname": "Sami",
  "email": "sksami4456@gmail.com"
}
```

## Technologies Used

- **Spring Boot 3.x**
- **Spring Data JPA**
- **MySQL 8.x**
- **Maven**
- **Java 17**

## License
This project is licensed under the MIT License.
