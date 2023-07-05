# user-service

The User Service handles user-related operations, such as user registration, authentication, and user retrieval. It provides endpoints for user registration, login, updating user information, retrieving user details, and more.

## Features

- User registration
- User login and authentication
- Updating user information
- Retrieving user details
- User access token generation and validation

## Getting Started

These instructions will get you a copy of the User Service up and running on your local machine for development and testing purposes.

## Technologies Used
- Java 17
- Spring Boot 3.1.0
- Maven 4.0.0
- PostgreSQL 15.3
  
## Dependencies

- [Spring Boot] 
- [Spring Web]
- [Spring Data JPA]
- [postgresql]
- [Spring Cloud]
- [Spring Cloud OpenFeign]
- [Spring Security]
- [JWT (JSON Web Tokens)]

### Prerequisites

- [Java SE Development Kit 17.0.5] (https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html)
- [Maven 4.0.0] (https://maven.apache.org/install.html)
- [Spring Boot CLI] (https://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/#getting-started-installing-the-cli) (Optional)

### Installation
1. Clone the repository:
```bash
git clone <repository-url>
```
2. Navigate to the project directory::
```bash
cd user-service
```
3. Open the application.properties file and configure the database connection details:
```
spring.datasource.url=jdbc:mysql://localhost:8086/users_db
spring.datasource.username=<database-username>
spring.datasource.password=<database-password>
```
4. Build the project using Maven:
```bash
cd user-service
```
5. Run the application:
```bash
mvn spring-boot:run
```
## API Documentation
The User Controller provides various endpoints for user operations. Here are some examples:

- POST /auth/token: Authenticates a user and returns an access token.
- GET /auth/users: Retrieves a list of all users.
- POST /auth/register: Registers a new user.
- PUT /auth/updateUser: Updates user information.
- GET /auth/users/{username}: Retrieves the details of a specific user.
- GET /auth/getid/{username}: Retrieves the ID of a user based on their username.
