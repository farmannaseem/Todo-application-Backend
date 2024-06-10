# Todo Application

This is a simple Todo application that allows users to manage their tasks. Users can sign up, sign in, create, update, delete, and search for todos. Authentication is implemented using JWT tokens.

## Features

- User Signup: Users can create an account by providing their name, email, and password.
- User Signin: Existing users can sign in with their email and password.
- Create Todo: Users can create new todos by providing a title and description.
- Get All Todos: Users can retrieve all their todos.
- Get Single Todo: Users can retrieve a single todo by its ID.
- Update Todo: Users can update a todo's title, description, pinned status, and favorite status.
- Delete Todo: Users can delete a todo.
- Search Todos: Users can search for todos based on a search string.

## Installation

To run this application locally, follow these steps:

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/Todo-application-Backend.git
    cd Todo-application-Backend
    ```

2. Install dependencies:

    ```bash
    npm install
    ```

3. Create a `.env` file in the root directory and add the following:

    ```env
    MONGO_URI=mongodb://127.0.0.1:27017/tododb
    JWT_SECRET=your_jwt_secret_key
    ```

4. Start the server:

    ```bash
    npm start
    ```

## API Endpoints

### User Authentication

- **Signup**
  - Method: `POST`
  - Endpoint: `/api/users/signup`
  - Request Body:
    ```json
    {
      "name": "John Doe",
      "email": "johndoe@example.com",
      "password": "password123"
    }
    ```
  - Response:
    ```json
    {
      "token": "your_jwt_token"
    }
    ```

- **Signin**
  - Method: `POST`
  - Endpoint: `/api/users/signin`
  - Request Body:
    ```json
    {
      "email": "johndoe@example.com",
      "password": "password123"
    }
    ```
  - Response:
    ```json
    {
      "token": "your_jwt_token"
    }
    ```

### Todos

(Include details for all other todo endpoints)

## Postman Collection

You can import the Postman collection from [this link](https://www.postman.com/your-collection-link).

## License

This project is licensed under the MIT License.
