# Microservices with Docker Compose and NGINX Reverse Proxy

This project demonstrates how to run two microservices 
(one in Go and one in Python/Flask) 
behind an NGINX reverse proxy using Docker Compose.

---

## Services

### 1. `service_1` – Go (Golang)
- Responds to:
  - `/ping` → returns status and service name
  - `/hello` → returns a welcome message

### 2. `service_2` – Python Flask
- Responds to:
  - `/ping` → returns status and service name
  - `/hello` → returns a welcome message

---

## Setup Instructions

### Prerequisites
- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/)

### To run the system:

```bash
docker compose up --build




Then visit in your browser:

http://localhost/service1/ping
http://localhost/service1/hello

http://localhost/service2/ping
http://localhost/service2/hello



