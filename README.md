# Task Manager API

This project implements a Task Manager API using Node.js and MongoDB.

## Setup

1. Clone the repository:

git clone <repository_url>



2. Install dependencies:

npm install



3. Set up environment variables:

Create a `.env` file in the root directory and add the following:

PORT=3000
MONGODB_URI=<your_mongodb_uri>



## Usage

### API Endpoints

#### 1. Create a Task

- **URL:** `/api/tasks`
- **Method:** POST
- **Request Body:**
  ```json
  {
    "title": "Task title",
    "description": "Task description"
  }

    Response: 201 Created


    {
      "_id": "task_id",
      "title": "Task title",
      "description": "Task description",
      "createdAt": "timestamp",
      "updatedAt": "timestamp"
    }

2. Update a Task

    URL: /api/tasks/:id
    Method: PUT
    Request Body:


{
  "title": "New task title",
  "description": "New task description"
}

Response: 200 OK


    {
      "_id": "task_id",
      "title": "New task title",
      "description": "New task description",
      "updatedAt": "timestamp"
    }

3. Delete a Task

    URL: /api/tasks/:id
    Method: DELETE
    Response: 204 No Content

4. Show all Tasks

    URL: /api/tasks
    Method: GET
    Response: 200 OK


    [
      {
        "_id": "task_id",
        "title": "Task title",
        "description": "Task description",
        "createdAt": "timestamp",
        "updatedAt": "timestamp"
      },
      {
        "_id": "task_id",
        "title": "Task title",
        "description": "Task description",
        "createdAt": "timestamp",
        "updatedAt": "timestamp"
      },
      ...
    ]

Contributors

    Nuhammed sobhi

Feel free to contribute by opening issues or pull requests.
