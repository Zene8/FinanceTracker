# Development Plan

This document outlines the development plan for the Finance Tracker application.

## Phase 1: Foundation (Authentication & Core Features)

*   **User Authentication:**
    *   **Backend:**
        *   Create a `User` entity with fields for username, password (hashed), and email.
        *   Implement Spring Security for user authentication and authorization.
        *   Create a REST controller for user registration and login.
        *   Implement JWT-based authentication to secure the API.
    *   **Frontend:**
        *   Create login and registration pages.
        *   Implement a service to handle user authentication.
        *   Store the JWT in local storage and include it in the headers of API requests.
*   **Transaction Enhancements:**
    *   **Backend:**
        *   Add a `type` field to the `Transaction` model (e.g., "income" or "expense").
        *   Add a `recurring` field to the `Transaction` model to indicate if it's a recurring transaction.
        *   Create a new entity for `RecurringTransaction` to store the schedule and other details.
    *   **Frontend:**
        *   Update the transaction form to include the new fields.
        *   Create a new page to manage recurring transactions.
*   **Dashboard:**
    *   **Frontend:**
        *   Create a dashboard page to display a summary of income vs. expenses, top spending categories, and recent transactions.

## Phase 2: Budgeting

*   **Backend:**
    *   Create a `Budget` entity with fields for category, amount, and month.
    *   Create a REST controller to manage budgets (CRUD operations).
    *   Implement a service to calculate the spending against the budget.
*   **Frontend:**
    *   Create a page to manage budgets.
    *   Display the budget and spending information on the dashboard and category pages.

## Phase 3: Reporting and Analytics

*   **Backend:**
    *   Create new API endpoints to provide data for reports (e.g., spending by category over time, income vs. expenses).
*   **Frontend:**
    *   Integrate a charting library (e.g., Chart.js) to create charts and graphs.
    *   Create a dedicated reporting page to display the charts.

## Phase 4: AI Features

*   **Backend:**
    *   **Automatic Transaction Categorization:**
        *   Implement a simple machine learning model (e.g., using a library like Weka or a simple keyword-based approach) to suggest a category for a new transaction based on its description.
        *   Create a new API endpoint to get category suggestions.
    *   **Spending Insights:**
        *   Implement a service to analyze spending patterns and generate insights (e.g., "You've spent 20% more on restaurants this month compared to last month").
        *   Create a new API endpoint to get spending insights.
*   **Frontend:**
    *   Integrate the category suggestion feature into the transaction form.
    *   Display the spending insights on the dashboard.
