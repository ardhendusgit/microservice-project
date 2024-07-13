# Emart E-Commerce Application

## Overview

This e-commerce application showcases a microservices architecture with the following components:

- NGINX as an API gateway.
- Client microservice for the front end (Angular).
- Emart API for backend services (NodeJS, MongoDB).
- Books API for book-related services (Java, MySQL).

Each service is designed to handle specific aspects of the application, ensuring a scalable and maintainable architecture.

## Steps

- Docker files written for each of the microservices denote the functioning of the processes within them, including the binaries they use and the ports they expose.
- Accordingly, docker images are built and orchestrated together using Docker-Compose.
- The official NGINX image is used to override the default nginx.conf with our own configuration which is then attached as a volume to make it survive container mortality.
