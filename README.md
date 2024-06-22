# README for Atlas T2 Docker project #3001

## Introduction
This repository contains Docker-related projects to practice and learn about containerization, Docker basics, and microservices architecture. Docker is a powerful tool that allows developers to package applications into containers—standalone executable packages that include everything needed to run the application, including the code, runtime, system tools, system libraries, and settings.

In this project, I will explore Docker by setting up a simple yet comprehensive infrastructure for an application. This includes understanding and implementing a reverse proxy, load balancing, and managing multiple services within Docker containers.

## High-Level Design
The project involves designing and deploying a multi-service application architecture using Docker. The setup includes:
- A reverse proxy/load balancer server acting as the entry point.
- Two API servers for handling backend logic.
- One front-end server for serving static content.

Traffic routing and load balancing are managed through a round-robin algorithm, ensuring even distribution of requests among the API servers.

## Prerequisites
- Install Docker Desktop on your local computer. Instructions can be found at [Docker's official website](https://www.docker.com/).
- Familiarize yourself with Docker concepts and basics.

## Tasks

### Task 0: Create Your First Docker Image
Create a Docker image based on the latest Ubuntu, update APT, and upgrade all installed software. The Docker image should, upon execution, echo "Hello, World!" in the terminal.

### Task 1: Back-end
Develop a backend service using Python3, Flask, and Docker. Ensure your Dockerfile is set up to handle Python dependencies via pip.

### Task 2: Front-end
Set up a front-end service that serves static content. Use Nginx as the web server and configure it to serve your static files. Also, set up a port for listening to incoming requests.

### Task 3: Connecting the Front-end and Back-end
Implement communication between the front-end and back-end services. Ensure that the front-end can dynamically display data fetched from the back-end service.

### Task 4: Making it Simpler with Docker Compose
Use Docker Compose to simplify the management of your multi-container application. Define your services, build contexts, Dockerfiles, images, and ports in a `docker-compose.yml` file.

### Task 5: Proxy Server
Implement a proxy server using JavaScript in your HTML file. This server will route requests to the appropriate service based on the request URL.

### Task 6: Scale Horizontally
Scale your application horizontally by adding multiple instances of your API server. Use Docker Compose to manage these instances.

## Repository Details
- **GitHub Repository**: atlas-softy-pinko-docker
- **Directory Structure**: Each task will have its own directory under the root of the repository.

---

By aligning the text with the rest of the document, you can avoid unintentional code block formatting in your Markdown documents.
