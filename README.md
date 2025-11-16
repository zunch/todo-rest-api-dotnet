# Todo REST API for ASP.NET Core

This repository contains a simple REST API for managing todos, built using ASP.NET Core. It supports basic CRUD operations such as creating, reading, updating, and deleting todo items.

---

## Features

- [x] Add a new todo item.
- [x] Retrieve all todos.
- [x] Get details of a specific todo by ID.
- [x] Update a todo item.
- [x] Delete a todo.
- [x] Mark a todo as complete/incomplete.

---

## Technology Stack

- **Programming Language**: C#
- **Framework**: ASP.NET Core
- **Database**: SQL Server
- **ORM**: Entity Framework Core

---

## API Documentation

### Endpoints

#### `POST /api/todos`
- **Purpose**: Create a new todo item.

#### `GET /api/todos`
- **Purpose**: Retrieve all todo items.

#### `GET /api/todos/{id}`
- **Purpose**: Retrieve a specific todo by ID.

#### `PUT /api/todos/{id}`
- **Purpose**: Update a todo item.

#### `DELETE /api/todos/{id}`
- **Purpose**: Delete a todo item by ID.

#### `PATCH /api/todos/{id}/complete`
- **Purpose**: Mark a todo as completed/incomplete.

---

## How to Run locally

1. Clone the repository:
   ```bash
   git clone https://github.com/zunch/todo-rest-api-dotnet.git
   ```

2. Open the project in Visual Studio or VS Code.

3. Apply migrations:
   ```bash
   dotnet ef migrations add InitialCreate
   dotnet ef database update
   ```

4. Run the application:
   ```bash
   dotnet run
   ```

5. Access the API via `https://localhost:5001/api/todos`. For Swagger, navigate to `https://localhost:5001/swagger`.

---

## License
This project is licensed under the MIT License.