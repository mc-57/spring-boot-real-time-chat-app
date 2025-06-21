A backend URL shortening service built with Spring Boot. 
Converts long URLs into short, manageable links and redirects users seamlessly. 
Includes expiration handling and Redis caching for high performance.

## Feature

- Shortens any valid URL
- Optional expiration time for each shortened URL
- Fast retrieval using Redis caching
- Redirects from short URL to original URL
- API testing enabled via Swagger UI
- Docker support for containerized deployment

## Tech Stack
- Java 17
- Spring Boot 3.4.3
- Spring Web, JPA, Validation
- MYSQL
- Redis (caching layer)
- springdoc-openapi (Swagger UI)
- Docker
- Junit & Mockito 

## Setup Instruction (Docker Only)

### Prerequisites

- `url-shortener-app.tar` (your Docker image)
- `docker-compose.yml` file (for container orchestration)
- Docker installed and running

### Load and Run

```bash
# 1. Load the Docker image
docker load -i url-shortener-app.tar

# 2. Start the application and Redis using docker-compose
docker-compose up
