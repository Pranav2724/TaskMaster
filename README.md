# TaskMaster: Collaborative Todo App with FastAPI
A Full Stack Web App simulating a basic list of todos supporting multiple users

## Features

- User authentication: Users can register, login, and logout.
- Todos management: Users can create, read, update, and delete todos.
- Password change: Users can change their passwords.

## Installation

1. Clone the repository:

   ```
   git clone https://github.com/your_username/your_repository.git
   ```

2. Install dependencies:

   ```
   pip install -r requirements.txt
   ```

## Usage

1. Run the FastAPI server:

   ```
   uvicorn main:app --reload
   ```

2. Access the web application at `http://localhost:8000`.

## Endpoints

- **/auth**: Authentication routes
  - **POST /auth/token**: Login to obtain access token
  - **GET /auth**: Login page
  - **POST /auth**: Handle user login
  - **GET /auth/logout**: Logout and clear access token
  - **GET /auth/register**: User registration page
  - **POST /auth/register**: Register a new user
- **/todos**: Todos routes
  - **GET /todos**: List all todos
  - **GET /todos/add-todo**: Todo creation page
  - **POST /todos/add-todo**: Create a new todo
  - **GET /todos/edit-todo/{todo_id}**: Todo edit page
  - **POST /todos/edit-todo/{todo_id}**: Update a todo
  - **GET /todos/delete/{todo_id}**: Delete a todo
  - **GET /todos/complete/{todo_id}**: Mark a todo as complete
- **/users**: User routes
  - **GET /users/edit-password**: User password change page
  - **POST /users/edit-password**: Change user password

## Folder Structure

- **main.py**: Main FastAPI application entry point.
- **auth.py**: Authentication routes and functions.
- **todos.py**: Todos routes and functions.
- **users.py**: User routes and functions.
- **database.py**: Database configuration and session management.
- **models.py**: SQLAlchemy models for database tables.
- **templates/**: HTML templates for rendering pages.
- **static/**: Static files like CSS, JavaScript, etc.

## Dependencies

- FastAPI: Web framework for building APIs with Python.
- SQLAlchemy: SQL toolkit and Object-Relational Mapping (ORM) library.
- Pydantic: Data validation and settings management library.
- Passlib: Password hashing library.
- Starlette: ASGI framework for building async applications.
- Jinja2: Templating engine for rendering HTML templates.

## Contributing

Contributions are welcome! Please feel free to submit issues or pull requests.

---
