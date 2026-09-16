# Library Management System

## Project Description

Library Management System is a full-stack web application for managing books, authors, categories, and book borrowings.

Users can register and log in using JWT authentication, browse available books, search and filter books, and manage their borrowings. Authorized users can perform actions according to their permissions.

The project consists of a Django REST Framework backend and a React frontend.

## Technologies

### Backend

* Python
* Django
* Django REST Framework
* PostgreSQL
* Simple JWT
* django-filter
* Pillow
* Swagger / OpenAPI
* Docker

### Frontend

* React
* Vite
* Axios
* React Router
* CSS

### Deployment

* Render
* GitHub

## Features

* User registration and authentication
* JWT authentication
* Access and refresh tokens
* Protected routes
* User-specific permissions
* Book CRUD operations
* Author management
* Category management
* Book borrowing
* Search books
* Filter books
* Order books
* Pagination
* Book cover images
* Responsive user interface
* Swagger/OpenAPI API documentation
* Docker support
* Production deployment on Render

## Main Models

* User
* Author
* Category
* Book
* Borrowing

### Relationships

* A Book belongs to one Author.
* An Author can have multiple Books.
* A Book belongs to one Category.
* A Category can contain multiple Books.
* A Borrowing belongs to one User.
* A Borrowing belongs to one Book.

The project uses ForeignKey relationships for these connections.

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/NinoKanashvili/Library.git
cd Library
```

### 2. Backend

```bash
cd Final_Project/backend
```

Create and activate a virtual environment if you are running the project without Docker:

```bash
python -m venv venv
source venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

### 3. Environment Variables

Create a `.env` file and configure the required environment variables.

Example:

```env
SECRET_KEY=your-secret-key
DEBUG=True
POSTGRES_DB=library_db
POSTGRES_USER=postgres
POSTGRES_PASSWORD=postgres
```

Do not commit `.env` files or secret keys to GitHub.

### 4. Run with Docker

From the project root:

```bash
docker compose up --build
```

The backend will be available at:

```text
http://localhost:8000/
```

The frontend will be available at:

```text
http://localhost:5173/
```

## API

The backend provides RESTful API endpoints for authentication, books, authors, categories, borrowings and other application functionality.

### Authentication

```text
POST /api/token/
POST /api/token/refresh/
```

### Books

```text
GET /api/books/
GET /api/books/{id}/
POST /api/books/
PUT /api/books/{id}/
PATCH /api/books/{id}/
DELETE /api/books/{id}/
```

### Authors

```text
GET /api/authors/
GET /api/authors/{id}/
POST /api/authors/
PUT /api/authors/{id}/
DELETE /api/authors/{id}/
```

### Categories

```text
GET /api/categories/
GET /api/categories/{id}/
POST /api/categories/
PUT /api/categories/{id}/
DELETE /api/categories/{id}/
```

### Borrowings

```text
GET /api/borrowings/
GET /api/borrowings/{id}/
POST /api/borrowings/
```

The exact available endpoints and request/response schemas can be viewed in the Swagger/OpenAPI documentation.

## API Documentation

Swagger/OpenAPI documentation is available through the Django REST API.

## Deployment

The project is deployed on Render.

### Backend

```text
https://library-2-pfn6.onrender.com
```

### Frontend

```text
https://library-3-eab8.onrender.com
```

The frontend communicates with the deployed Django REST API using Axios.

## Live Demo

**Library Management System:**

https://library-3-eab8.onrender.com

## GitHub Repository

https://github.com/NinoKanashvili/Library
