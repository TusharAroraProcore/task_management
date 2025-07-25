# task_management
# Task Management Application

A full-stack task management system with a Spring Boot backend, PostgreSQL database, and React frontend. The project is containerized using Docker Compose for easy local development.

## Features
- Task CRUD operations
- Commenting on tasks
- Activity feed
- Responsive React UI
- RESTful API (Spring Boot)
- PostgreSQL database
- Dockerized frontend, backend, and database

## Project Structure
```
task_management/
├── demo/                # Spring Boot backend
├── task-ui-app/         # React frontend
├── docker-compose.yml   # Multi-container orchestration
```

## Getting Started

### Prerequisites
- Docker & Docker Compose
- (Optional) Node.js & npm (for frontend development)
- (Optional) Java 17+ & Maven (for backend development)

### Running with Docker Compose
```sh
docker-compose up -d
```
- Frontend: http://localhost:3001
- Backend: http://localhost:8080
- PostgreSQL: localhost:5432 (user: postgres, password: postgres)

### Building Backend JAR (if needed)
```sh
cd demo
./mvnw clean package
```

### Running Frontend Locally (optional)
```sh
cd task-ui-app
npm install
npm start
```

## Environment Variables
See `docker-compose.yml` for all service environment variables.

## License
MIT
