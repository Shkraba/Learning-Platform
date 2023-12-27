# Language Exchange and Learning Platform

**Study Project**

This repository contains the source code for a study project focused on building a Language Exchange and Learning Platform. The platform is designed to facilitate language exchange between users, providing features for messaging, user management, content sharing, and real-time notifications.

## Project Structure

The project is organized into four main microservices:

1. **Messaging Service**
2. **User Service**
3. **Content Service**
4. **Notification Service**

Each service is built using .NET 8 and C# following the principles of Domain-Driven Design (DDD). The chosen technologies and architectural patterns for each service are as follows:

### 1. Messaging Service

- **Communication Mechanism:** Kafka
- **Architectural Patterns:** CQRS, Event Sourcing
- **Read Database:** MS SQL
- **Write Database:** MongoDB
- **Manually implemented mediator

### 2. User Service

- **Communication Mechanism:** RabbitMQ
- **Architectural Patterns:** CQRS, Event Sourcing
- **Write Database:** PostgreSQL
- **Read Database:** Redis
- **Library:** MediatR
- **Data Access:** Dapper

### 3. Content Service (More info coming soon)

- **Search Engine:** Elasticsearch
- **Database:** MongoDB

### 4. Notification Service (More info coming soon)

- **Real-Time Communication:** SignalR
- **Database:** MS SQL

## Getting Started

### Prerequisites

- [.NET 8 SDK](https://dotnet.microsoft.com/download/dotnet/8.0)
- [Docker](https://www.docker.com/)

### Running the Services

1. **Messaging Service:**
   - Navigate to the `MessagingService` directory
   - Run `docker-compose up` to start Kafka and other dependencies
   - Start the Messaging Service project

2. **User Service:**
   - Navigate to the `UserService` directory
   - Run `docker-compose up` to start RabbitMQ and other dependencies
   - Start the User Service project

3. **Content Service:**
   - Navigate to the `ContentService` directory
   - Start the Content Service project

4. **Notification Service:**
   - Navigate to the `NotificationService` directory
   - Start the Notification Service project

## Contributing

Feel free to contribute to the project by opening issues, submitting pull requests, or suggesting improvements. This is a study project, and collaboration is encouraged to enhance the learning experience.

## License

This project is licensed under the [MIT License](LICENSE).
