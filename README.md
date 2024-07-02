# Project Setup with Nginx and Astro

This repository contains a setup for serving a static website generated using Astro.js with Nginx in a Docker container.

## Getting Started

To run this project locally, follow these steps:

### Prerequisites

- Docker installed on your machine ([Docker Installation Guide](https://docs.docker.com/get-docker/))

### Build and Run the Docker Container

1. **Clone the repository:**

2. **Build the Docker image:**

   ```bash
   docker build -t astro-nginx .
   ```

3. **Run the Docker container:**

   ```bash
   docker run -p 8080:80 astro-nginx
   ```

4. **Access the application:**

   Open your web browser and navigate to [http://localhost:8080](http://localhost:8080)

### Notes

- The Dockerfile includes instructions to set up an Nginx server to serve the Astro.js generated static files.
- The `nginx.conf` file is configured to handle clean URLs without file extensions using Nginx.
