Production Simulator – Phase 1

Overview
This phase demonstrates the basic request–response lifecycle of the Production Simulator. It focuses on handling JSON requests, converting them into Java objects, processing them through the service layer, storing incidents, and returning a JSON response to the client.

Workflow
Client Request (JSON)

The client sends a JSON payload representing an incident.

Spring Conversion

Spring automatically converts the JSON into a CreateIncidentRequest object.

This is mapped to the Incident domain object.

Controller Layer

The IncidentController receives the CreateIncidentRequest.

It delegates the processing to the service layer.

Service Layer

The IncidentService creates a new Incident object.

The incident is stored in a HashMap (acting as an in-memory database for Phase 1).

Response Handling

The stored incident is converted back into JSON.

The JSON response is sent back to the client.

Data Flow

Client (JSON Request)
        ↓
Spring → CreateIncidentRequest / Incident
        ↓
Controller receives object
        ↓
Service creates Incident object
        ↓
Incident stored in HashMap
        ↓
Response → JSON
        ↓
Client receives JSON Response
