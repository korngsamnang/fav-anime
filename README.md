# Favnime (MERN Stack Project)

## Introduction

This is a MERN (MongoDB, Express.js, React.js, Node.js) stack project that has been Dockerized for easy deployment and
management.

## Prerequisites

Before you begin, make sure you have the following installed on your machine:

- Docker: [Get Docker](https://docs.docker.com/engine/install/)
- Docker Compose: [Get Docker Compose](https://docs.docker.com/compose/install/)
- Recommended: (Install Docker Desktop which includes
  both Docker Engine and Docker Compose)

## Running the Application

1. Clone the repository to your local machine:

    ```bash
    git clone https://github.com/korngsamnang/favnime
    cd favnime
    ```

2. Create a `.env` file in the project root and configure the necessary environment variables. You can use the
   provided `.env.example` file as a template.

3. Build and run the Docker containers:

    ```bash
   docker compose up
    ```

   This command will build the Docker images and start the containers for the MongoDB, Express.js, React.js, and Node.js
   components.

4. Once the containers are up and running, you can access the application at:

    - Frontend: [http://localhost:5173](http://localhost:5173)
    - Backend: [http://localhost:8000](http://localhost:8000)

5. Keep project in sync when make changes

    ```bash
   docker compose watch
    ```

   This command will watch for changes in the frontend and backend folders and rebuild the Docker images and restart the
   containers.

## Stopping the Application

To stop the application and remove the containers, run the following command in the project root:

  ```bash
   docker compose down
   ```

## Additional Information

- Customize the configuration by modifying the `compose.yml` file and other relevant configuration files.
- For production deployment, make sure to secure your environment variables and update the Docker Compose file
  accordingly.

Happy coding!
