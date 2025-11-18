# ShopoSphere: Distributed Order Fulfillment Platform

This repository models a **Distributed Order Fulfillment Platform** for a multinational retailer, built as a set of independent Spring Boot microservices. 

## Project Structure

The **ShopoSphere platform** is structured as a microservice with the following components:

## Service Descriptions

### 1. `shoposphere-parent`
- **Description**: Parent POM that manages dependency versions for all services in the platform.

### 2. `shoposphere-config-server`
- **Description**: Centralized configuration management for all services using Spring Cloud Config Server.

### 3. `shoposphere-eureka-server`
- **Description**: Eureka Server for service discovery and registration. All services register here.

### 4. `shoposphere-api-gateway`
- **Description**: API Gateway built with Spring Cloud Gateway, routing external requests, performing JWT validation, rate-limiting, and basic request transformations.

### 5. `shoposphere-auth-service`
- **Description**: Authentication service responsible for issuing and validating JWT tokens for users.

### 6. `shoposphere-order-service`
- **Description**: Manages customer orders and the order lifecycle.

### 7. `shoposphere-pricing-service`
- **Description**: Provides product pricing information for orders.

### 8. `shoposphere-inventory-service`
- **Description**: Manages stock levels and inventory data for products.

### 9. `shoposphere-shipping-service`
- **Description**: Handles shipping and tracking of customer orders.

### 10. `shopsphere-shared`
- **Description**: Shared libraries containing common DTOs, models, and exceptions used across all services.

### 11. `shopsphere-zipkin-server`
- **Description**: Self-hosted Zipkin server for distributed tracing of requests across services.
