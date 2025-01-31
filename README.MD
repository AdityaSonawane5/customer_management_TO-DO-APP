# Customer Management System

A Spring Boot web application for managing customer information with CRUD operations.

## Features
- 📝 Create new customers
- 📋 View all customers in a table format
- ✏️ Update existing customer information
- 🗑️ Delete customers
- 📱 Responsive web interface

## Tech Stack
### Backend
- ☕ Java 17
- 🚀 Spring Boot 3.4.1
- 🗄️ Spring Data JPA
- 💾 MySQL Database

### Frontend
- 🌐 HTML5
- 🎨 CSS3
- ⚡ JavaScript (Vanilla)
- 🔗 RESTful API Integration

## Project Structure
```
src/
├── main/
│   ├── java/
│   │   └── com/example/Project01/
│   │       ├── controller/
│   │       │   └── CustomerController.java
│   │       ├── entity/
│   │       │   └── Customer.java
│   │       ├── repository/
│   │       │   └── CustomerRepository.java
│   │       ├── service/
│   │       │   └── CustomerService.java
│   │       └── Project01Application.java
│   └── resources/
│       ├── static/
│       │   └── index.html
│       └── application.properties
```

## Setup & Installation
### Prerequisites
- ✅ Java 17 or higher
- ✅ MySQL Server
- ✅ Maven

### Database Configuration
Create a MySQL database named `customer_db` and update `application.properties` with your database credentials:
```properties
spring.datasource.url=jdbc:mysql://localhost:3306/customer_db
spring.datasource.username=Your_Username
spring.datasource.password=Your_Password
```

### Build & Run
Run the following commands:
```sh
mvn clean install
mvn spring-boot:run
```

### Access Application
Open your browser and navigate to: [http://localhost:8080](http://localhost:8080)

## API Endpoints
| Method | URL                 | Description                |
|--------|---------------------|----------------------------|
| GET    | `/api/customers`      | 📄 Get all customers         |
| POST   | `/api/customers`      | 🆕 Create a new customer     |
| PUT    | `/api/customers/{id}` | ✏️ Update customer by ID     |
| DELETE | `/api/customers/{id}` | 🗑️ Delete customer by ID     |

## 🤝 Contributing
Feel free to fork this repository and submit pull requests for any improvements.

## 📜 License
This project is licensed under the **MIT License**.
