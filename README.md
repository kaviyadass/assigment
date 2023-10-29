# Role Management API

This is a Spring Boot REST API for managing user roles with the following capabilities:

- Create, Find, Update and Delete
- API access  using Spring Security

## API Endpoints

### Create USER
- **HTTP Method**: POST
- **Endpoint**: `/api/User
- **Description**: Create a new user
- **Request Body**:
  ```json
  {
      "id" : "int",
      "name": "string",
      "address" : "string",
      "email" : "string",
      "contactnumber" : "string"
        
  }

### Find Role
- **HTTP Method**: GET
- **Endpoint**: /api/roles/{UserId}
- **Description**: Retrieve a user by ID


### Update Role
- **HTTP Method**: PUT
- **Endpoint**: /api/roles/{roleId}
- **Description**: Update an existing role by ID
- Request Body:
  ```json
  {
      "id" : "int",
      "name": "string",
      "address" : "string",
      "email" : "string",
      "contactnumber" : "string"
        
  }
### Delete Role
- **HTTP Method**: DELETE
- **Endpoint**: /api/roles/{roleId}
- **Description**: Delete a user by ID

## Database
The API uses a PostgreSQL database to store role information.

## Testing with Postman
- You can use Postman to test the API by sending HTTP requests to the specified endpoints. 
- Make sure to include a valid JWT token in the request headers for authentication.

## Setup
- Clone this repository.

   ```bash
   git clone https://github.com/kaviyadass/assignment
- Make sure you have PostgreSQL installed and create a database.
- Configure the database connection in application.properties.
- Run the application using Spring Boot or your favorite IDE.
