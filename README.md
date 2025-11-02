# Spring Boot React SQLite Project

This project is a full-stack application that uses Spring Boot for the backend and React for the frontend, with SQLite as the database.

## Project Structure

```
spring-boot-react-sqlite
├── server                # Backend Spring Boot application
│   ├── pom.xml          # Maven configuration file
│   ├── src
│   │   ├── main
│   │   │   ├── java
│   │   │   │   └── com
│   │   │   │       └── example
│   │   │   │           └── app
│   │   │   │               ├── Application.java
│   │   │   │               ├── controller
│   │   │   │               │   ├── HealthController.java
│   │   │   │               │   └── UserController.java
│   │   │   │               ├── service
│   │   │   │               │   └── UserService.java
│   │   │   │               ├── repository
│   │   │   │               │   └── UserRepository.java
│   │   │   │               └── model
│   │   │   │                   └── User.java
│   │   │   └── resources
│   │   │       ├── application.properties
│   │   │       └── data.sql
│   │   └── test
│   │       └── java
│   │           └── com
│   │               └── example
│   │                   └── app
│   │                       └── ApplicationTests.java
├── client                # Frontend React application
│   ├── package.json      # npm configuration file
│   ├── tsconfig.json     # TypeScript configuration file
│   ├── public
│   │   └── index.html    # Main HTML file
│   └── src
│       ├── index.tsx     # Entry point for React application
│       ├── App.tsx       # Main component of the React application
│       └── components
│           └── ExampleComponent.tsx # Example component
├── .gitignore            # Git ignore file
└── README.md             # Project documentation
```

## Getting Started

### Prerequisites

- Java 11 or higher
- Maven
- Node.js and npm
- SQLite

### Backend Setup

1. Navigate to the `server` directory.
2. Run `mvn clean install` to build the Spring Boot application.
3. Run the application using `mvn spring-boot:run`.

### Frontend Setup

1. Navigate to the `client` directory.
2. Run `npm install` to install the dependencies.
3. Start the React application using `npm start`.

### API Endpoints

- `GET /api/health` - Check the health status of the application.
- `GET /api/users/{id}` - Retrieve user information by ID.
- `POST /api/users` - Create a new user.

### Database

The application uses SQLite as the database. The initial data can be found in `server/src/main/resources/data.sql`.

## License

This project is licensed under the MIT License.