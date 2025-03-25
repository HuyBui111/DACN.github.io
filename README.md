# Rental Management System

## Project Overview
The Rental Management System is a web-based platform designed to facilitate the management of rental rooms efficiently. It allows property owners to manage tenants, track payments, monitor utility usage, and generate financial reports.

## Technologies Used
- **Spring Boot** – Backend framework for building the RESTful API.
- **MySQL** – Database management system.
- **RESTful API** – For efficient data exchange between client and server.
- **JWT (JSON Web Token)** – Secure authentication and authorization mechanism.
- **VNPay API** – Integration for online payments.
- **MailService** – Email notifications for invoices and important updates.

## Features
### 1. Authentication & Authorization
- Secure user authentication using JWT.
- Role-based access control for admins and tenants.

### 2. Email Notifications
- Automatic email invoicing for tenants.
- Notifications for upcoming payments and contract renewals.

### 3. Online Payment Support
- VNPay integration for deposits and monthly rent payments.
- Transaction history tracking.

### 4. Customer Portal
- Room booking feature.
- View invoices and make payments online.

### 5. Revenue & Reporting
- Track rental income, tenant deposits, and overall profit.
- Generate financial reports for better investment tracking.

### 6. Management Features
- **Room Management** – Add, update, or delete rooms.
- **Bill Management** – Generate and send monthly bills.
- **Customer Management** – Store and manage tenant details.
- **Electricity & Water Tracking** – Monitor and bill utilities usage.

## Installation & Setup
### Prerequisites
- Java 17+
- MySQL Database
- Maven
- Postman (for API testing)

### Steps to Run the Project
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repository-url
   ```
2. Navigate to the project directory:
   ```bash
   cd rental-management-system
   ```
3. Configure database connection in `application.properties`:
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/rental_db
   spring.datasource.username=root
   spring.datasource.password=yourpassword
   ```
4. Install dependencies:
   ```bash
   mvn clean install
   ```
5. Run the application:
   ```bash
   mvn spring-boot:run
   ```
6. Access the API via Postman or frontend at `http://localhost:8080`.

## API Endpoints
| Endpoint | Method | Description |
|----------|--------|-------------|
| `/api/auth/register` | POST | Register a new user |
| `/api/auth/login` | POST | Authenticate user and return JWT |
| `/api/rooms` | GET | Retrieve list of rooms |
| `/api/payments` | POST | Process rental payments via VNPay |
| `/api/invoices` | GET | View all invoices |

## Contribution Guidelines
1. Fork the repository.
2. Create a new branch: `git checkout -b feature-branch`.
3. Commit changes: `git commit -m "Add new feature"`.
4. Push to branch: `git push origin feature-branch`.
5. Open a Pull Request.

## License
This project is licensed under the MIT License.

---
**Author:** [Your Name]  
**Contact:** [Your Email]

