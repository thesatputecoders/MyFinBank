# My Fin Bank

My Fin Bank is a microservices-based banking application built using Spring Boot for the backend and Angular for the frontend. This project demonstrates a complete banking solution with various services handling different aspects of banking operations.

## Project Structure

```
My-Fin-Bank
├── backend
│   ├── config-server          # Spring Cloud Config Server
│   ├── discovery-server       # Eureka Discovery Server
│   ├── customer-service       # Customer management service
│   ├── account-service        # Account management service
│   └── transaction-service     # Transaction management service
├── frontend
│   └── angular-app            # Angular frontend application
└── docker-compose.yml         # Docker configuration for the application
```

## Technologies Used

- **Backend:**
  - Spring Boot
  - Spring Security
  - Spring Cloud Config
  - Eureka Discovery Server
  - OpenFeign
  - JWT Authentication
  - MySQL Database

- **Frontend:**
  - Angular
  - TypeScript
  - HTML/CSS

## Features

- **Customer Service:** Handles customer registration and information management.
- **Account Service:** Manages account details and balance inquiries.
- **Transaction Service:** Facilitates deposit, withdrawal, and fund transfer operations.
- **Centralized Configuration:** Utilizes Spring Cloud Config Server for managing configuration properties.
- **Service Discovery:** Implements Eureka Server for service registration and discovery.
- **Secure APIs:** Protects APIs using JWT authentication.
- **Inter-Service Communication:** Uses OpenFeign for seamless communication between services.

## Getting Started

### Prerequisites

- Java 11 or higher
- Node.js and npm
- MySQL Database
- Docker (optional)

### Backend Setup

1. Navigate to the `backend` directory.
2. Build the project using Maven:
   ```
   mvn clean install
   ```
3. Configure the MySQL database in the `application.yml` files of each service.
4. Start the services using Docker or run them individually.

### Frontend Setup

1. Navigate to the `frontend/angular-app` directory.
2. Install the dependencies:
   ```
   npm install
   ```
3. Start the Angular application:
   ```
   ng serve
   ```

## Contributing

Contributions are welcome! Please feel free to submit a pull request or open an issue for any suggestions or improvements.

## License

This project is licensed under the MIT License. See the LICENSE file for details.