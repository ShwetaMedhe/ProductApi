# Product Management API

A RESTful Product Management API built using ASP.NET Core 8 following Clean Architecture principles. The project supports CRUD operations, JWT Authentication, API Versioning, AutoMapper, FluentValidation, Serilog logging, and SQL Server.

## Features

- CRUD Operations
- JWT Authentication & Authorization
- Role-Based Authorization
- API Versioning
- Entity Framework Core
- SQL Server
- Repository Pattern
- Clean Architecture
- AutoMapper
- FluentValidation
- Serilog Logging
- Swagger UI
- Docker Support
- Unit Testing (xUnit & Moq)

## Tech Stack

- ASP.NET Core 8
- C#
- SQL Server
- Entity Framework Core
- JWT
- AutoMapper
- FluentValidation
- Serilog
- Swagger
- Docker
- xUnit
- Moq

## Project Structure

```
ProductApi
│
├── API
├── Application
├── Domain
├── Infrastructure
├── Application.Tests
├── docker-compose.yml
└── ProductApi.sln
```

## Getting Started

### Clone Repository

```bash
git clone https://github.com/ShwetaMedhe/ProductApi.git
```

# Authentication APIs

| Method | Endpoint | Description |
|---------|----------|-------------|
| POST | /api/v1/Auth/login | Login |
| POST | /api/v1/Auth/refresh-token | Generate New Access Token |
| POST | /api/v1/Auth/logout | Logout |

---

# Product APIs

| Method | Endpoint | Description |
|---------|----------|-------------|
| GET | /api/v1/Products | Get All Products |
| GET | /api/v1/Products/{id} | Get Product By Id |
| POST | /api/v1/Products | Create Product |
| PUT | /api/v1/Products/{id} | Update Product |
| DELETE | /api/v1/Products/{id} | Delete Product |

---

# Query Parameters

| Parameter | Description |
|-----------|-------------|
| pageNumber | Current Page Number |
| pageSize | Number of Records |

Example

```
GET /api/v1/Products?pageNumber=1&pageSize=5
```

---

# Error Response

Example

```json
{
  "statusCode": 500,
  "message": "An unexpected error occurred."
}
```

---

# Swagger

After running the project

```
https://localhost:5001/swagger
```

Use the **Authorize** button and paste the JWT Bearer Token.

---


## Authentication

JWT Authentication is used.

Roles:

- Admin
- User

- # Logging

Serilog is used for logging.

Log files are generated inside

```

## Output Screenshots

Project output screenshots are available in the **Screenshots** folder.

## Author

Shweta Medhe



GitHub:
https://github.com/ShwetaMedhe
