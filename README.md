# All is Well Pharma - Pharmaceutical Management System

## Overview
The **All is Well Pharma** Pharmaceutical Management System is a robust and user-friendly application designed to enable pharmacists to efficiently manage, update, and track drug information. The system automates critical workflows, ensuring data accuracy, improved operational efficiency, and compliance with industry standards.

---

## Features

- **Drug Inventory Management:** Track available drugs, manage stock levels, and update inventory efficiently.
- **Purchase and Sales Records:** Maintain detailed records of purchases and sales, enabling effective auditing and reporting.
- **Expiry Tracking:** Automatically track expiration dates to prevent the sale of expired drugs.
- **Supplier Management:** Store and manage supplier details for streamlined procurement.
- **Search and Filter Functionality:** Quickly retrieve specific drug or transaction data using advanced search filters.
- **Secure Authentication:** Role-based authentication for secure access.

---

## Technologies Used

### Backend:
- **Java**
- **Spring Boot**
- **RESTful APIs**

### Database:
- **MySQL**

### Frontend (optional):
- **Thymeleaf** (if applicable)
- **HTML/CSS/JavaScript**

### Tools:
- **Maven** for dependency management
- **Lombok** for boilerplate code reduction
- **Postman** for API testing
- **H2 Console** (for testing purposes)

---

## Setup and Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/all-is-well-pharma.git
   cd all-is-well-pharma
   ```

2. Configure the database:
   - Update the `application.properties` file with your database credentials.
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/pharma_db
   spring.datasource.username=your-username
   spring.datasource.password=your-password
   spring.jpa.hibernate.ddl-auto=update
   ```

3. Build the project using Maven:
   ```bash
   mvn clean install
   ```

4. Run the application:
   ```bash
   mvn spring-boot:run
   ```

5. Access the application:
   - API endpoints: `http://localhost:8080/api`
   - Frontend (if applicable): `http://localhost:8080`

---

## Project Structure

```plaintext
src/main/java
├── com.alliswellpharma
│   ├── controller    # REST Controllers
│   ├── model         # Entity classes
│   ├── repository    # JPA Repositories
│   ├── service       # Business Logic
│   └── dto           # Data Transfer Objects

src/main/resources
├── static            # Static files (CSS, JS, images)
├── templates         # Thymeleaf templates (if applicable)
├── application.properties
```

---

## API Endpoints

| Endpoint                       | Method | Description                        |
|--------------------------------|--------|------------------------------------|
| `/api/drugs`                   | GET    | Get all drugs                     |
| `/api/drugs/{id}`              | GET    | Get drug by ID                    |
| `/api/drugs`                   | POST   | Add a new drug                    |
| `/api/drugs/{id}`              | PUT    | Update drug information           |
| `/api/drugs/{id}`              | DELETE | Delete a drug                     |
| `/api/suppliers`               | GET    | Get all suppliers                 |
| `/api/suppliers`               | POST   | Add a new supplier                |

---

## Future Enhancements

- Integration with third-party APIs for real-time drug availability.
- Enhanced analytics and reporting dashboards.
- Multi-language support.
- Mobile application integration.

---

## License

This project is licensed under the [MIT License](LICENSE).

---

## Contributing

Contributions are welcome! Please fork this repository and submit a pull request with detailed information about your changes.

---

## Acknowledgments

Special thanks to the development team and mentors for their guidance and support in building this application.
