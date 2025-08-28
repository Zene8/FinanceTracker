# FinanceTracker

A web application to track personal finances.

## Project Description

FinanceTracker is a full-stack web application designed to help users manage their finances. It features a Spring Boot backend that provides a REST API for managing financial data, and a Blazor WebAssembly frontend for a rich user interface. The application allows users to categorize their expenses and manage personal financial records.

## Tech Stack

*   **Backend:** Java 17, Spring Boot 3.5.5, Spring Data JPA, H2 Database, Maven
*   **Frontend:** .NET 8, Blazor

## Development Environment Setup

### Prerequisites

*   Java JDK 17 or later
*   Apache Maven
*   .NET 8 SDK

### Backend

1.  **Navigate to the backend directory:**
    ```bash
    cd backend
    ```
2.  **Run the Spring Boot application:**
    ```bash
    mvn spring-boot:run
    ```
    The backend server will start on `http://localhost:8080`.

### Frontend

1.  **Navigate to the frontend directory:**
    ```bash
    cd frontend
    ```
2.  **Run the Blazor application:**
    ```bash
    dotnet run
    ```
    The frontend application will be accessible at the address provided in the console (usually `http://localhost:5000` or `https://localhost:5001`).

## Testing

### Backend

To run the backend tests, navigate to the `backend` directory and run:

```bash
mvn test
```

### Frontend

There are currently no automated tests for the frontend. Future development will include adding unit and integration tests for the Blazor components.

## Deployment

### Backend

1.  **Package the application:**
    Navigate to the `backend` directory and run:
    ```bash
    mvn package
    ```
    This will create a JAR file in the `target` directory.
2.  **Run the application:**
    ```bash
    java -jar target/financetracker-0.0.1-SNAPSHOT.jar
    ```

### Frontend

1.  **Publish the application:**
    Navigate to the `frontend` directory and run:
    ```bash
    dotnet publish -c Release
    ```
2.  **Deploy the contents:**
    Deploy the contents of the `bin/Release/net8.0/publish/wwwroot` directory to a static web hosting service.

## Future Development

*   **Transaction Management:** Add functionality to create, edit, and delete financial transactions.
*   **User Authentication:** Implement user authentication and authorization to secure user data.
*   **Reporting and Analytics:** Develop features for generating financial reports and visualizing data with charts.
*   **Database Integration:** Replace the in-memory H2 database with a persistent database like PostgreSQL or MySQL.
*   **Enhanced UI/UX:** Improve the user interface and user experience with a more modern design and responsive layout.
*   **Comprehensive Testing:** Increase test coverage for both the backend and frontend.
