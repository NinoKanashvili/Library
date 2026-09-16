# Library Management System

## Project Name

Library Management System

## Project Description

Library Management System is a web application for managing books in a digital library.

Users can register and log in, browse books, search and filter them, and borrow available books. The application provides a simple and responsive interface for managing and viewing library information.

## Technologies

* Python
* Django
* Django REST Framework
* React
* PostgreSQL
* Axios
* React Router
* Docker
* Render
* Swagger / OpenAPI

## Features

* User registration and login
* JWT authentication
* Browse books
* Search books
* Filter books
* Sort books
* Pagination
* Borrow books
* User-specific borrowing information
* Protected routes
* Responsive design
* API documentation with Swagger

## Installation

Clone the repository:

```bash
git clone https://github.com/NinoKanashvili/Library.git
cd Library
```

Run the project with Docker:

```bash
docker compose up --build
```

The frontend runs on:

```text
http://localhost:5173
```

The backend runs on:

```text
http://localhost:8000
```

## API

Main API endpoints:

### Authentication

```text
POST /api/token/
POST /api/token/refresh/
```

### Books

```text
GET /api/books/
POST /api/books/
GET /api/books/{id}/
PUT /api/books/{id}/
DELETE /api/books/{id}/
```

### Authors

```text
GET /api/authors/
POST /api/authors/
GET /api/authors/{id}/
PUT /api/authors/{id}/
DELETE /api/authors/{id}/
```

### Categories

```text
GET /api/categories/
POST /api/categories/
GET /api/categories/{id}/
PUT /api/categories/{id}/
DELETE /api/categories/{id}/
```

### Borrowings

```text
GET /api/borrowings/
POST /api/borrowings/
GET /api/borrowings/{id}/
```

## Deployment

The project is deployed on Render.

Backend:

https://library-2-pfn6.onrender.com/api

Frontend:

https://library-3-eab8.onrender.com

## Live Demo

https://library-3-eab8.onrender.com
