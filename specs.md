# Task Tracker Specification

## Goal

Build a REST API for task management.

## Features

### Create Task

Input:

{
    "title": "Learn Copilot"
}

Rules:

- Title required
- Maximum 100 characters

Response:

{
    "id": 1,
    "title": "Learn Copilot",
    "completed": false
}

---

### Get Tasks

GET /tasks

Returns all tasks.

---

### Update Task

PATCH /tasks/:id

Can update:

- title
- completed

---

### Delete Task

DELETE /tasks/:id

Removes task.

---

## Non Functional Requirements

- Node.js
- Express
- In-memory storage
- Jest unit tests
- REST standards
