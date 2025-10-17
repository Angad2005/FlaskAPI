# Flask API Sandbox 🧪

This is my first project using Flask to build a simple RESTful API. It's a lightweight sandbox for prototyping and testing basic API endpoints and learning the fundamentals of backend development in Python.

## About The Project

This project was created as a hands-on learning exercise to understand the core concepts of building an API. The main goal was to create a minimal, functioning backend that can handle basic HTTP requests and respond with JSON data.

It serves as a personal playground to explore:

- Basic routing in Flask
- Handling GET and POST requests
- Sending and receiving JSON payloads
- Setting up a simple development environment

## Getting Started

Follow these steps to get a local copy up and running.

### Prerequisites

Make sure you have Python and pip installed on your system.

- Python 3.x
- pip

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/your-username/your-repository-name.git

2. **Navigate to the project directory**

   ```bash
   cd your-repository-name

3. **Create and activate a virtual environment**

- On macOS/Linux:

   ```bash
   python3 -m venv venv
   source venv/bin/activate

- On Windows:

   ```bash
   python -m venv venv
   .\venv\Scripts\activate

4. **Install the required packages**

   ```bash
   pip install -r requirements.txt
(Note: To generate the requirements.txt file, run pip freeze > requirements.txt after installing Flask.)

Running the Application
Start the Flask development server

Bash

flask run
The API will be running at http://127.0.0.1:5000

Usage
You can test the endpoints using a tool like curl or Postman.

GET /api/hello
Returns a simple welcome message.

Request:

Bash

curl http://127.0.0.1:5000/api/hello
Response:

JSON

{
  "message": "Hello! This is my first Flask API."
}
POST /api/echo
Echoes back the JSON data sent in the request body.

Request:

Bash

curl -X POST \
  -H "Content-Type: application/json" \
  -d '{"name": "User", "data": "Some sample data"}' \
  http://127.0.0.1:5000/api/echo
Response:

JSON

{
  "received_data": {
    "name": "User",
    "data": "Some sample data"
  },
  "status": "success"
}
Built With
Python

Flask

License
Distributed under the MIT License. See LICENSE for more information.
