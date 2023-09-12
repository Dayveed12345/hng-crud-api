

# HNGX CRUD API README

Welcome to the HNG CRUD API project! This repository contains the source code for our CRUD API. Follow the instructions below to set up and interact with the API locally.

## Getting Started

### Prerequisites

Before you begin, make sure you have the following software installed on your system:

- PHP (v7.3.0 or higher)
- Composer (v2.0.0 or higher)
- Node.js (v14.0.0 or higher)
- npm (v6.0.0 or higher)
- PGSQL (v5.7.0 or higher)

### Installation

1. Clone the project repository:

   ```bash
   git clone https://github.com/Dayveed12345/hng-crud-api.git
   ```

2. Navigate to the project folder:

   ```bash
   cd hng-crud-api
   ```

3. Install PHP dependencies using Composer:

   ```bash
   composer install
   ```

4. Install JavaScript dependencies using npm:

   ```bash
   npm install
   ```

5. Create a copy of the `.env.example` file and save it as `.env`:

   ```bash
   cp .env.example .env
   ```

6. Generate an application key:

   ```bash
   php artisan key:generate
   ```

7. Open the `.env` file and configure your database connection settings.

### Running the API

1. Run database migrations to create the necessary database tables:

   ```bash
   php artisan migrate
   ```

   If your project includes seed data, you can also run database seeders:

   ```bash
   php artisan db:seed
   ```

2. Start the Laravel development server:

   ```bash
   php artisan serve
   ```

   The API will be accessible at `http://localhost:8000` by default.

## Using the CRUD API

You can use standard HTTP methods (GET, POST, PUT, DELETE) to interact with the CRUD API.

- **Create**: Use a POST request to create a new resource.
- **Read**: Use a GET request to retrieve one or more resources.
- **Update**: Use a PUT request to update an existing resource.
- **Delete**: Use a DELETE request to remove a resource.

Here are some example API endpoints:

- Create a new resource: `POST http://localhost:8000/api`
- Read all resources: `GET http://localhost:8000/api`
- Read a specific resource: `GET http://localhost:8000/api/{user_id}`
- Update a resource: `PUT http://localhost:8000/api/{user_id}`
- Delete a resource: `DELETE http://localhost:8000/api/{user_id}`

Please refer to the API documentation for more details on using specific endpoints and data formats.

## UML Diagrams
You can view the UML diagrams for this project [here](https://hng-uml-diagram.netlify.app/).
