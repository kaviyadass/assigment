# User Management API

This is a Spring Boot REST API for managing user  with the following capabilities:

- Create, Find, Update and Delete
- API access  using Spring Security
- 
## Table of Contents

- [User Management API](#user-management-api)
  - [API Endpoints](#api-endpoints)
    - [Create USER](#create-user)
    - [Find User](#find-user)
    - [Update User](#update-user)
    - [Delete User](#delete-user)
  - [Database](#database)
  - [Testing with Postman](#testing-with-postman)
  - [Setup](#setup)


## API Endpoints

### Create USER
- **HTTP Method**: POST
- **Endpoint**: /api/v1/User
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

### Find User
- **HTTP Method**: GET
- **Endpoint**: /api/v1/User{UserId}
- **Description**: Retrieve a user by ID


### Update User
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
### Delete User
- **HTTP Method**: DELETE
- **Endpoint**: /api/v1/User{roleId}
- **Description**: Delete a user by ID

## Database
The API uses a PostgreSQL database to store role information.

## Testing with Postman
- You can use Postman to test the API by sending HTTP requests to the specified endpoints. 
- Make sure to include a valid JWT token in the request headers for authentication.

## Setup
- Clone this repository.

   ```bash
   git clone https://github.com/kaviyadass/assigment.git
- Make sure you have PostgreSQL installed and create a database.
- Configure the database connection in application.properties.
- Run the application using Spring Boot or your favorite IDE on local server **9090** .
