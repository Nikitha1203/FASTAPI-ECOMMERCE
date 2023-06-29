# FASTAPI-ECOMMERCE
# Item Management Application

This application allows you to manage items through CRUD (Create, Read, Update, Delete) operations. It provides a set of API endpoints to interact with the items stored in the system.

## Features

- Create: Add new items to the system.
- Read: Retrieve information about existing items.
- Update: Modify the details of existing items.
- Delete: Remove items from the system.

## Technologies Used

- Backend Framework: [FastAPI](https://fastapi.tiangolo.com/)
- Database: [PostgreSQL](https://www.postgresql.org/)
- API Documentation: [Swagger UI](https://swagger.io/tools/swagger-ui/)
- Authentication: JWT (JSON Web Tokens)

## Getting Started

### Prerequisites

- Python 3.9 or higher
- PostgreSQL database
- Virtual environment (optional, but recommended)

### Installation

1. Clone the repository: `git clone https://github.com/your-username/item-management-app.git`
2. Navigate to the project directory: `cd item-management-app`
3. Create and activate a virtual environment (optional): 
   - Linux/Mac: `python3 -m venv venv && source venv/bin/activate`
   - Windows: `python -m venv venv && venv\Scripts\activate`
4. Install the required dependencies: `pip install -r requirements.txt`
5. Set up the database connection:
   - Update the database configuration in the `config.py` file.
6. Run the application: `python main.py`
7. Access the API documentation: `http://localhost:8000/docs`

## Usage

Once the application is up and running, you can use any HTTP client (e.g., cURL, Postman) to interact with the API endpoints.

### Create an Item

Send a POST request to `/items` with the item details in the request body.

### Read an Item

Send a GET request to `/items/{item_id}` to retrieve information about a specific item.

### Update an Item

Send a PUT request to `/items/{item_id}` with the updated item details in the request body.

### Delete an Item

Send a DELETE request to `/items/{item_id}` to remove an item from the system.

## Authentication

Some routes may require authentication to access. You need to obtain a JWT token by sending a POST request to `/login` with valid credentials. Include the token in the `Authorization` header for authenticated routes (Bearer Token).

## License

This project is licensed under the [MIT License](LICENSE).
