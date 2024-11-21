
# MERN Docker App

This project demonstrates how to containerize a full-stack MERN (MongoDB, Express, React, Node.js) application using Docker. The repository provides all necessary configurations to build, run, and manage the app with Docker containers.

## Features

- **MongoDB:** Database container for storing application data.
- **Express.js:** Backend framework to handle API endpoints.
- **React:** Frontend framework for the user interface.
- **Node.js:** Server-side runtime for backend operations.
- **Docker:** Containerization for consistent environments across development and production.

## Prerequisites

Ensure you have the following installed on your system:

- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/install/)

## Getting Started

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/chouaib-skitou/mern-docker-app.git
   cd mern-docker-app
   ```

2. **Build and Start Containers:**
   ```bash
   docker-compose up --build
   ```

3. **Access the Application:**
   - Frontend: `http://localhost:3000`
   - Backend API: `http://localhost:5000`
   - MongoDB: `localhost:27017`

## Project Structure

```plaintext
mern-docker-app/
├── backend/        # Node.js + Express backend
├── frontend/       # React frontend
├── docker-compose.yml
├── Dockerfile      # Dockerfile for backend
└── README.md
```

## Docker Setup

- **Backend Container:**
  - Built using `Dockerfile` in the `backend` directory.
  - Exposes port `5000` for API requests.
  
- **Frontend Container:**
  - Built using `Dockerfile` in the `frontend` directory.
  - Exposes port `3000` for the React app.

- **MongoDB Container:**
  - Defined in `docker-compose.yml`.
  - Uses the official `mongo` Docker image.

## Useful Commands

- **Stop Containers:**
  ```bash
  docker-compose down
  ```

- **Rebuild Containers:**
  ```bash
  docker-compose up --build
  ```

- **Check Running Containers:**
  ```bash
  docker ps
  ```

## Contributing

Feel free to fork this repository and submit pull requests. Contributions are always welcome!

---

### Author

[Chouaib Skitou](https://github.com/chouaib-skitou) - Software Engineer
