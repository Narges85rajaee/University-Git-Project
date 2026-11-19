
# System Architecture Diagram

## Student Task Management System

```mermaid
flowchart TD
    A[Client / User] -->|HTTP Request| B[REST API]
    B -->|Process Request| C[Backend Server]
    C -->|Read / Write Data| D[(Database)]
    D --> C
    C -->|HTTP Response| B
    B --> A
```

## Architecture Description

- Client sends requests to the API.
- REST API receives and processes requests.
- Backend Server handles business logic.
- Database stores Users and Tasks data.
- Server sends responses back to the Client.
