# Finance Tracker

A full-stack web application for personal finance management, built with a Spring Boot backend and a Blazor frontend.

## Table of Contents

- [About the Project](#about-the-project)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
- [Roadmap](#roadmap)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## About the Project

This project is a comprehensive suite for managing personal finances. It allows users to track their income and expenses, create budgets, and gain insights into their spending habits. The application is designed to be user-friendly and intuitive, with a clean and modern interface.

### Built With

*   **Backend:**
    *   [Spring Boot](https://spring.io/projects/spring-boot)
    *   [Spring Data JPA](https://spring.io/projects/spring-data-jpa)
    *   [Maven](https://maven.apache.org/)
*   **Frontend:**
    *   [Blazor](https://dotnet.microsoft.com/apps/aspnet/web-apps/blazor)
    *   [.NET 8](https://dotnet.microsoft.com/download/dotnet/8.0)
*   **Database:**
    *   [H2 Database](https://www.h2database.com/html/main.html) (for development)
    *   [PostgreSQL](https://www.postgresql.org/) (for production)

## Getting Started

To get a local copy up and running follow these simple steps.

### Prerequisites

*   Java 17 or higher
*   .NET 8 SDK
*   Node.js (for frontend dependencies)

### Installation

1.  **Clone the repo**
    ```sh
    git clone https://github.com/your_username/FinanceTracker.git
    ```
2.  **Backend Setup**
    ```sh
    cd backend
    mvn spring-boot:run
    ```
3.  **Frontend Setup**
    ```sh
    cd frontend
    dotnet watch run
    ```

## Usage

Once the application is running, you can access it at `http://localhost:5000`. You can start by creating categories for your expenses, adding people, and then tracking your transactions.

## Roadmap

See the [DEVELOPMENT_PLAN.md](DEVELOPMENT_PLAN.md) file for a detailed look at the future of the project.

## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

## License

Distributed under the MIT License. See `LICENSE` for more information.

## Contact

Your Name - your_email@example.com

Project Link: [https://github.com/your_username/FinanceTracker](https://github.com/your_username/FinanceTracker)