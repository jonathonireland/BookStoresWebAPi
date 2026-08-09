# BookStoresWebAPi

A starter bookstore REST API built with ASP.NET Core 8, Entity Framework Core, SQL Server, and Swagger/OpenAPI.

## Current Foundation

- ASP.NET Core controller-based API structure
- HTTPS redirection
- Authorization middleware ready for protected endpoints
- Swagger/OpenAPI generation and interactive development UI
- Entity Framework Core SQL Server packages
- Nullable reference types and implicit global usings

## Technologies

- C#
- .NET 8
- ASP.NET Core Web API
- Entity Framework Core 8
- SQL Server
- Swagger / Swashbuckle

## Run Locally

### Prerequisites

- [.NET 8 SDK](https://dotnet.microsoft.com/download/dotnet/8.0)
- SQL Server when persistence is configured

### Start the API

```bash
dotnet restore
dotnet run
```

When running in the Development environment, use the Swagger URL printed in the console to inspect the available endpoints.

## Development Direction

This repository establishes the web API host and required persistence packages. Natural next steps include:

- Define book, author, and store domain models
- Add an Entity Framework Core `DbContext`
- Configure the database connection through environment-specific settings
- Add migrations and seed data
- Implement asynchronous CRUD controllers
- Add DTOs, validation, and mapping
- Add authentication and authorization policies
- Add unit and integration tests

## Configuration Guidance

Store local connection strings in user secrets or development-only configuration and use environment variables in deployed environments. Do not commit database credentials.
