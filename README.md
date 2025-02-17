# Krishi - A Smart Farming Assistance System

## Overview
Krishi is a web-based application designed to assist farmers in making informed decisions at various stages of the farming lifecycle. The system provides location-based services, weather forecasts, market prices, and government scheme details, helping farmers increase productivity and optimize resources efficiently.

## Features
- **User Authentication**: Farmers and laborers can register and log in to access personalized services.
- **Farmer's Profile**: Maintain farmer-related data such as land details and preferred crops.
- **Laborer's Profile**: Store and manage labor-related information.
- **Weather Updates**: Real-time weather forecasts to aid in farming decisions.
- **Market Connectivity**: Enables farmers to connect with markets, suppliers, and contractors.
- **Government Schemes**: Provides information on various agricultural schemes and subsidies.
- **Nearby Services**: Locate farming-related services like pesticide shops and labor contractors.

## Tech Stack
- **Backend**: Java, Spring Boot
- **Frontend**: HTML, CSS, JavaScript
- **Database**: MySQL
- **Version Control**: Git, GitHub

## System Requirements
- Java 11 or later
- Spring Boot 3.x
- MySQL Database
- Maven or Gradle

## Installation Guide
### 1. Clone the Repository
```sh
 git clone <GitHub Repository URL>
 cd krishi
```

### 2. Configure Database
- Create a database in MySQL:
```sql
 CREATE DATABASE krishi_db;
```
- Update `application.properties` with MySQL credentials:
```properties
spring.datasource.url=jdbc:mysql://localhost:3306/krishi_db
spring.datasource.username=root
spring.datasource.password=yourpassword
spring.jpa.hibernate.ddl-auto=update
```

### 3. Build and Run the Application
```sh
 mvn clean install
 mvn spring-boot:run
```

### 4. Access the Application
- API Documentation (if enabled): `http://localhost:8080/swagger-ui/`
- Web Portal: `http://localhost:8080/`

## API Endpoints
| Endpoint | Method | Description |
|----------|--------|-------------|
| `/api/auth/register` | POST | Register a new user |
| `/api/auth/login` | POST | Authenticate user |
| `/api/weather` | GET | Fetch weather updates |
| `/api/farmers` | GET | Retrieve farmer profiles |
| `/api/markets` | GET | Find nearby markets |

## Contribution
1. Fork the repository.
2. Create a feature branch (`git checkout -b feature-branch`).
3. Commit changes (`git commit -m 'Added new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a Pull Request.

## License
This project is open-source and available under the MIT License.

## Contact
For further queries, reach out via [GitHub Issues](<GitHub Repository URL>) or email at `support@krishi.com`.

---

_"Empowering Farmers with Technology"_ 🌱

