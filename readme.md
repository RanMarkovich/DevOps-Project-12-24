# Hello World Flask Application

This is a simple Flask application that returns "Hello, World!" when accessed.

## Prerequisites

- Python 3.11 or higher
- `pip` (Python package installer)
- Docker (optional, for running via Docker)
- PyCharm (optional, for running via PyCharm)

## Running the Application Locally

### Using PyCharm

1. **Open the Project**: Open the project in PyCharm.
2. **Install Dependencies**:
   - Open the terminal in PyCharm.
   - Navigate to the `app` directory: `cd app`
   - Run: `pip install -r requirements.txt`
3. **Run the Application**:
   - Right-click on `hello_world.py` and select `Run 'hello_world'`.
   - The application will start, and you can access it at `http://127.0.0.1:5000`.

### Using Docker

1. **Build the Docker Image**:
   - Open a terminal.
   - Navigate to the project directory.
   - Run: `docker build -t hello-world-flask -f app/Dockerfile .`
2. **Run the Docker Container**:
   - Run: `docker run -p 5000:5000 hello-world-flask`
   - The application will start, and you can access it at `http://127.0.0.1:5000`.

## Application Structure

- `app/hello_world.py`: The main Flask application file.
- `app/requirements.txt`: The file containing the required Python packages.
- `app/Dockerfile`: The Dockerfile for building the Docker image.

## Accessing the Application

Once the application is running, open your web browser and go to `http://127.0.0.1:5000`. You should see the message "Hello, World!".