# React Task Manager

A simple task manager built with React, Express, and PostgreSQL.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Contributing](#contributing)
- [License](#license)

## Overview

This project is a basic task manager application developed using React for the frontend, Express for the backend, and PostgreSQL for the database. Users can add tasks with due dates, mark them as completed, and delete tasks. Deleted tasks are moved to a separate table for reference.

## Features

- Add tasks with due dates
- Mark tasks as completed
- Delete tasks (moved to a separate "deletedTasks" table)
- View deleted tasks for reference

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/react-task-manager.git
Install dependencies for both the frontend and backend:

bash
Copy code
cd react-task-manager
cd frontend
npm install
cd ../backend
npm install
Set up the PostgreSQL database:

Create a .env file in the backend directory with the following content:

makefile
Copy code
DATABASE_URL=your_postgresql_database_url
PORT=your_preferred_port
Replace your_postgresql_database_url with the connection URL for your PostgreSQL database.

Replace your_preferred_port with the port you want the server to run on.

Run the backend and frontend servers:

bash
Copy code
# In the backend directory
npm start

# In the frontend directory
npm start
Usage
Access the application at http://localhost:3000 in your browser.
Add tasks using the input form.
Double-click on a task to mark it as completed and move it to the deleted tasks list.
API Endpoints
Tasks
GET /api/tasks: Get all tasks.
GET /api/tasks/:id: Get a specific task by ID.
POST /api/tasks: Add a new task.
DELETE /api/tasks/:id: Delete a task by ID.
Deleted Tasks
GET /api/deletedTasks: Get all deleted tasks.
GET /api/deletedTasks/:id: Get a specific deleted task by ID.
POST /api/deletedTasks: Add a new deleted task.
DELETE /api/deletedTasks/:id: Delete a deleted task by ID.
Contributing
Contributions are welcome! Feel free to open issues or submit pull requests.

License
This project is licensed under the MIT License.

css
Copy code

Make sure to customize any placeholders and adapt the content to fit the specifics of your project.
