# Spring boot microservices
E-Commerce Microservices Architecture 🚀

This project implements a scalable, event-driven e-commerce system using Spring Boot 3, Spring Cloud, and Kafka. It follows Domain-Driven Design (DDD) principles and is structured into multiple independent microservices, each handling a specific business domain.

🛠 Architecture Overview

The system consists of the following microservices:

1️⃣ API Gateway
Acts as a single entry point for all client requests
Routes requests to respective microservices (/customers, /products, /orders)
Ensures load balancing and security
2️⃣ Customer Service
Manages customer data stored in MongoDB
Handles customer-related API endpoints
3️⃣ Product Service
Manages the product catalog
Stores product details in a relational database
4️⃣ Order Service
Processes order placement
Stores order data and interacts with Payment Service
5️⃣ Payment Service
Handles payment transactions
Sends payment confirmation asynchronously via Kafka
6️⃣ Notification Service
Listens for order and payment events from Kafka
Sends notifications to users
Stores notification data in MongoDB
7️⃣ Infrastructure Components
Eureka Server: Service discovery for dynamic microservice registration
Config Server: Centralized configuration management
Kafka & Zookeeper: Enables asynchronous communication between microservices
Zipkin: Distributed tracing for monitoring service interactions
🔗 Communication Between Services

Synchronous calls through API Gateway (REST)
Asynchronous messaging via Kafka for event-driven workflows
Service discovery via Eureka for dynamic scaling
🔧 Tech Stack

✅ Spring Boot 3, Spring Cloud (Config, Eureka, Gateway)
✅ Apache Kafka & Zookeeper (Event-driven architecture)
✅ Docker & Docker Compose (Containerization)
✅ MongoDB & Relational Databases (Data storage)
✅ Keycloak (Authentication & Authorization)
✅ Zipkin (Tracing & Logging)


📌 Features Implemented

✔ Scalable and modular microservices architecture
✔ Event-driven communication using Kafka
✔ Secure authentication using Keycloak
✔ Centralized configuration for easy deployment
✔ Distributed tracing with Zipkin
