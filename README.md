# 💬 Real-Time Chat Application

A simple, secure real-time chat application build with Spring Boot,
WebSocket(STOMP), and MySQL. This project showcases real-time messaging,
persistent chat history, read receipts, and chat room management.

## 🚀 Features

- User Registration & Login: JWT-based authentication with Spring Security.
- Protected Endpoints: Secure REST and WebSocket channels so only authenticated users can participate.
- Chat Room Management: Create or join chat rooms.
- Real-time Message: Bidirectional messaging using STOMP over WebSocket.
- Message Persistence: Store and load chat history from MySQL.
- Read Receipts: Messages show a blue indicator when delivered. Recipients click a message to
  mark it as read, turning the indicator green so senders see it's been seen in real time.
- Minimal Frontend Client: HTML/JavaScript demo using SockJS & STOMP.js.

## 🧰 Tech Stack

- Backend: Java 17, Spring Boot
- Security: Spring Security, JWT
- Real-time: Spring WebSocket, STOMP
- Persistence: Spring Data JPA, MYSQL
- Containerization: Docker, Docker Compose
- Frontend (Demo):HTML, JavaScript (SockJS & STOMP.js)

## 🐳 Docker Image

You can use the pre-built Docker image directly from Docker Hub:

🔗 [michellec07/spring-boot-real-time-chat-app](https://hub.docker.com/r/michellec07/spring-boot-real-time-chat-app)

## ⚙️ Setup Instruction (Docker Only)

### 📦 Prerequisites

Ensure you have the following installed:

- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/install/)

Clone this repository to get the necessary files:

- `docker-compose.yml` — defines the backend and MySQL containers  
- `init.sql` — initializes the MySQL database with sample data

### ▶️ Run the Application

```bash
# Step 1: Pull the pre-built backend image from Docker Hub
docker pull michellec07/spring-boot-real-time-chat-app:latest

# Step 2: Start backend and MySQL containers
docker-compose up -d
```

### 📺 Access the Application

Visit [http://localhost:8080/client-chat.html](http://localhost:8080/client-chat.html) in your browser to access the Swagger UI for testing the API.
