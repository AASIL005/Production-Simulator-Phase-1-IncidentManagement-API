# Production Simulator - Phase 1: Incident Management API

This phase focuses on building the core backend structure of the Production Incident Simulator.

The goal was to create a REST API capable of creating and retrieving incidents while understanding the basic flow of a Spring Boot application.

## Features Implemented

- Incident Model
- REST Controller
- Service Layer
- Create Incident API
- Get All Incidents API
- In-Memory Storage using HashMap

## API Endpoints

### Create Incident

POST /incidents

### Get All Incidents

GET /incidents

## Learning Outcomes

- Spring Boot Project Structure
- REST API Development
- Dependency Injection
- Controller-Service Architecture
- Request and Response Handling
- In-Memory Data Storage

## Architecture

Client
    ↓
Controller
    ↓
Service
    ↓
HashMap Storage

## Example Use Case

A user creates an incident through the API. The request is processed by the controller, handled by the service layer, and stored in memory for retrieval.

## Key Takeaway

This phase established the foundation of the application and introduced the core request flow used throughout the project.
