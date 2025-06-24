# 🏦 Simple Banking Application (Flask + SQLite + Docker)

## 📌 Objective
The goal of this project is to demonstrate a basic banking application that allows users to:

- Create new accounts

- Check account balance

- Deposit and withdraw money

- View transaction statements

This lightweight app showcases fundamental backend development concepts using Flask, SQLite, and HTML templating — ideal for learning or teaching beginner-level web development and database operations.


## 🛠 Tech Stacks
- Backend: Python 3, Flask

- Database: SQLite

- Frontend: HTML (rendered with Flask templates)

- Containerization: Docker

- Browser-based UI: Runs locally via Flask routes


## 🔄 Steps Included

## 1. Database Initialization

- Two tables are created:

- accounts: stores user info and balance

- transactions: logs deposits and withdrawals

## 2. Web Interface Functionalities

- `/create`: Create a new bank account

- `/balance`: Check the balance using account ID

- `/deposit`: Deposit money to an account

- `/withdraw`: Withdraw money after checking balance

- `/statement`: View recent transactions for an account

## 3. Flask App Execution

- All functionalities are wrapped under Flask routes.

- Database operations are securely performed using SQLite.

- HTML content is rendered via Flask’s render_template_string.

## 4. Docker Integration

- Dockerfile provided to containerize the app.

- Exposes port 5002 to run on http://localhost:5002.


## 📊 Key Insights
- Demonstrates CRUD operations using Python + SQLite.

- Emphasizes form handling and routing in Flask.

- Shows basic transaction logic, such as preventing withdrawals if balance is insufficient.

- UI is beginner-friendly and functional, rendered using inline HTML.

- Portable: Easily deployable using Docker.


## 🚀 How to Run (Locally using Docker)
```
# Build Docker image
docker build -t banking-app .

# Run the container
docker run -d -p 5002:5002 banking-app
```
- Access it at: http://localhost:5002


## 📁 Project Structure
```
.
├── app.py          # Main Flask application
├── Dockerfile      # Container configuration
├── bank.db         # SQLite database (auto-created on first run)
```

✅ Additional Notes
- Educational Use: Ideal for beginner students learning web development and SQL.

- Extendable: Can be enhanced with login, encryption, or using a production database like PostgreSQL.

- Security Note: This is a demo app; sensitive data handling and authentication are not included.

