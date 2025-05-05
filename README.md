# Softy Pinko Docker Project

This project focuses on containerization using Docker to build a scalable web application infrastructure. Through a series of progressive tasks, you'll create and connect multiple containers to form a complete application stack with a reverse proxy, load balancer, API servers, and front-end server.

## Project Overview

In this project, you will:

1. Create basic Docker images
2. Build a Flask-based API server
3. Set up a static content front-end server using Nginx
4. Connect front-end and back-end services
5. Implement a reverse proxy with Nginx
6. Configure load balancing for horizontal scaling

## Architecture

The final architecture will include:
- A reverse proxy server (acting as the entry point)
- A load balancer (distributing traffic between API servers)
- Multiple API servers (providing backend functionality)
- A front-end server (serving static content)

## Prerequisites

- Docker Desktop installed on your local machine
- Basic understanding of Docker concepts
- Familiarity with web servers and proxies

## Tasks

0. **Create Your First Docker Image**: Build a basic Ubuntu-based Docker image
1. **Back-end**: Create a Flask API server
2. **Front-end**: Set up a static web server with Nginx
3. **Connecting Front-end and Back-end**: Enable communication between containers
4. **Docker Compose**: Simplify deployment with docker-compose
5. **Proxy Server**: Implement a reverse proxy for routing requests
6. **Scale Horizontally**: Configure load balancing across multiple API servers

## Resources

- [Docker Documentation](https://docs.docker.com/)
- [Docker Cheatsheet](https://docs.docker.com/get-started/docker_cheatsheet.pdf)
- [Nginx Documentation](https://nginx.org/en/docs/)
- [Flask Documentation](https://flask.palletsprojects.com/)

## Project Structure

```
holbertonschool-softy-pinko-docker/
│
├── task0/
│   └── Dockerfile
│
├── task1/
│   ├── Dockerfile
│   └── api.py
│
├── task2/
│   ├── back-end/
│   │   ├── Dockerfile
│   │   └── api.py
│   └── front-end/
│       ├── Dockerfile
│       ├── softy-pinko-front-end/
│       └── softy-pinko-front-end.conf
│
├── task3/
│   ├── back-end/
│   │   ├── Dockerfile
│   │   └── api.py
│   └── front-end/
│       ├── Dockerfile
│       ├── softy-pinko-front-end/
│       └── softy-pinko-front-end.conf
│
├── task4/
│   ├── back-end/
│   │   ├── Dockerfile
│   │   └── api.py
│   ├── front-end/
│   │   ├── Dockerfile
│   │   ├── softy-pinko-front-end/
│   │   └── softy-pinko-front-end.conf
│   └── docker-compose.yml
│
├── task5/
│   ├── back-end/
│   │   ├── Dockerfile
│   │   └── api.py
│   ├── front-end/
│   │   ├── Dockerfile
│   │   ├── softy-pinko-front-end/
│   │   └── softy-pinko-front-end.conf
│   ├── proxy/
│   │   ├── Dockerfile
│   │   └── proxy.conf
│   └── docker-compose.yml
│
└── task6/
    ├── back-end/
    │   ├── Dockerfile
    │   └── api.py
    ├── front-end/
    │   ├── Dockerfile
    │   ├── softy-pinko-front-end/
    │   └── softy-pinko-front-end.conf
    ├── proxy/
    │   ├── Dockerfile
    │   └── proxy.conf
    ├── docker-compose.yml
    └── 2-api-servers.txt
```
