# PharmaApplication

## Overview
PharmaApplication is a **Spring Boot-based Pharmaceutical Management System** that allows administrators and pharmacists to manage medicines, track orders, and handle secure user authentication. The system is designed to optimize pharmacy operations by ensuring secure transactions, proper inventory management, and seamless order processing.

## Features
- **User Authentication & Role-Based Access**
  - Secure login using **Spring Security (JWT/OAuth2)**.
  - Role management for **Admins, Pharmacists, and Customers**.

- **Medicine Inventory Management**
  - Add, update, and delete medicines.
  - View stock availability and track expiration dates.

- **Order & Transaction Processing**
  - Customers can place orders and track their purchase history.
  - Pharmacists can manage stock availability and process orders.

- **RESTful API Development**
  - Exposes endpoints for **user authentication, inventory management, and order processing**.

- **Database Integration**
  - Uses **Spring Data JPA & Hibernate** for efficient database management.
  - Supports **MySQL/PostgreSQL**.

- **Deployment & DevOps**
  - Maven-based project for easy dependency management.
  - Can be **Dockerized & deployed** on cloud platforms like AWS/GCP/Azure.

## Tech Stack
- **Backend:** Java, Spring Boot, Hibernate, JPA
- **Security:** Spring Security (JWT, OAuth2)
- **Database:** MySQL/PostgreSQL
- **Build & Deployment:** Maven, Docker, AWS/Azure

## Installation & Setup
1. **Clone the Repository**
   ```sh
   git clone https://github.com/your-username/PharmaApplication.git
   cd PharmaApplication
   ```

2. **Configure the Database** (MySQL/PostgreSQL)
   - Update `application.properties` with database credentials:
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/pharma_db
   spring.datasource.username=root
   spring.datasource.password=yourpassword
   ```

3. **Build & Run the Application**
   ```sh
   mvn clean install
   mvn spring-boot:run
   ```

4. **API Endpoints**
   - Swagger documentation available at: `http://localhost:8080/swagger-ui.html`
   - Example API endpoints:
     - `POST /auth/login` - User authentication
     - `GET /medicines` - Get available medicines
     - `POST /orders` - Place an order

## Future Enhancements
- Implement **Swagger API Documentation** for better API visibility.
- Add **Email Notifications** for order confirmations.
- Convert to **Microservices Architecture** for scalability.

## License
This project is licensed under the [MIT License](LICENSE).

---

Feel free to contribute or raise issues if you find any improvements!

