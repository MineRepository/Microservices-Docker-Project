# Microservices Docker Project: Signup, Login, and Quiz

This project consists of three independent frontend microservices: `signup-service`, `login-service`, and `quiz-service`. Each service is built using NGINX to serve static HTML pages and is containerized using Docker.

---

## Project Structure
project/
├── docker-compose.yml
├── signup-service/
│   ├── Dockerfile
│   ├── public/
│   │   └── index.html
├── login-service/
│   ├── Dockerfile
│   ├── public/
│   │   └── index.html
├── quiz-service/
│   ├── Dockerfile
│   ├── public/
│   │   └── index.html


---

## Microservices Overview

1. **Signup Service**
   - Provides the frontend for user signup.
   - Includes a button to navigate to the login page.

2. **Login Service**
   - Provides the frontend for user login.
   - Includes a button to navigate to the quiz page.

3. **Quiz Service**
   - Provides the frontend for a simple quiz page.

Each service runs independently, serving its respective HTML page through an NGINX container.

---

## Prerequisites

- Docker installed on your system.
- Docker Compose installed.

---

## Usage

### 1. Clone the Repository

```bash
git clone <repository-url>
cd project

Build and Start the Services:
docker-compose up --build

This will:
Build Docker images for each microservice.
Start containers for the signup-service, login-service, and quiz-service.

HOW TO ACCESS: 
Signup Page: http://localhost:8080
Login Page: http://localhost:8081
Quiz Page: http://localhost:8082
