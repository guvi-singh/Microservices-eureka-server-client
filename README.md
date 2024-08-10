
# Microservices Discovery Server and Client

## Overview

The **Microservices-discovery-server-client** project demonstrates the use of a Discovery Server (via Netflix Eureka) for service discovery in a microservices architecture. This setup enhances the previous implementation by removing hardcoded service addresses and ports, allowing for dynamic service discovery. The project includes three core services: **Order Service**, **Inventory Service**, and **Product Service**.

## Features

- **Discovery Server**: Acts as a centralized service registry for managing service instances.
- **Eureka Clients**: Each service registers itself with the Discovery Server, enabling dynamic discovery.
- **Dynamic Scaling**: Easily run multiple instances of each service without manual port tracking.
- **Improved Flexibility**: Remove hardcoding of service addresses and ports, facilitating smoother operations and scalability.

## Project Structure

- **discovery-server**: Configures the Discovery Server for service registration and discovery.
- **order-service**: Service that processes orders and communicates with Inventory Service to check stock levels.
- **inventory-service**: Manages inventory and provides availability information to Order Service.
- **product-service**: Handles product information and interacts with Order Service for product details.

## Setup

1. **Start Discovery Server**: Launch the Discovery Server application. It will be accessible at `http://localhost:8761/`.
2. **Run Client Services**: Start the Order Service, Inventory Service, and Product Service applications. Each service will automatically register with the Discovery Server.

## Benefits

Integrating a Discovery Server for service discovery provides:
- **Scalability**: Easily manage multiple instances of services without manual configuration.
- **Flexibility**: Dynamically discover services without hardcoded addresses and ports.
- **Simplified Management**: Automatically handle service instances and their availability.

## Dependencies

- **Spring Boot 3.3.2**
- **Spring Cloud 2023.0.0**

## Acknowledgments

Special thanks to SaiUpadhyayula for invaluable assistance in the development and setup of this project.

