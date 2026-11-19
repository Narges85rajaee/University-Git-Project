# Chapter 3 - API Contract

## Project Name
Student Task Management System

## Resources
- Users
- Tasks

## Description
This project provides an API for managing students and their tasks.

## API Endpoints

### Users Resource

| Method | Endpoint | Description |
|---|---|---|
| GET | /api/users | Get all users |
| GET | /api/users/1 | Get user by ID |
| POST | /api/users | Create a new user |
| PUT | /api/users/1 | Update user |
| DELETE | /api/users/1 | Delete user |

### Tasks Resource

| Method | Endpoint | Description |
|---|---|---|
| GET | /api/tasks | Get all tasks |
| GET | /api/tasks/1 | Get task by ID |
| POST | /api/tasks | Create a new task |
| PUT | /api/tasks/1 | Update task |
| DELETE | /api/tasks/1 | Delete task | 

## HTTP Status Codes

| Status Code | Meaning | Usage |
|---|---|---|
| 200 OK | Successful request | Data retrieved or updated successfully |
| 201 Created | Resource created | New user or task created |
| 204 No Content | Successful deletion | User or task deleted |
| 400 Bad Request | Invalid request | Required data is missing or invalid |
| 404 Not Found | Resource not found | User or task does not exist |
| 500 Internal Server Error | Server error | Unexpected server problem |

## API Response Examples

### Successful Response (200 OK)

{
  "message": "Request successful",
  "data": []
}

### Created Response (201 Created)

{
  "message": "Resource created successfully"
}

### Error Response (404 Not Found)

{
  "error": "Resource not found"
}
