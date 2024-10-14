# My Docker Flask App

This is a basic Python Flask application containerized with Docker. The application returns "Hello, Docker!" when accessed through a web browser.

## Requirements

To run this project, you'll need:

- [Docker](https://www.docker.com/get-started)

## Project Structure

```
my-docker-project/
│
├── app.py              # Main Flask application
├── Dockerfile          # Docker configuration
├── requirements.txt    # Application dependencies
└── README.md           # Project documentation
```

## Getting Started

Follow these steps to run the project in a Docker container.

### 1. Clone the Repository

```bash
git clone https://github.com/Vrana710/my-docker-project.git
cd my-docker-project
```

### 2. Build the Docker Image

Run the following command to build the Docker image for the Flask app:

```bash
docker build -t my-flask-app .
```

### 3. Run the Docker Container

Start the Flask application inside a Docker container by running:

```bash
docker run -p 5000:5000 my-flask-app
```

### 4. Access the Application

Open your browser and navigate to:

```
http://localhost:5000
```

You should see the message "Hello, Docker!".

## Using Docker Compose (Optional)

If you prefer using Docker Compose, you can use the provided `docker-compose.yml` file to run the app.

```bash
docker-compose up
```

This will build the image (if not already built) and run the application.

### Stopping the Application

To stop the Docker container, use `Ctrl + C` in the terminal if you're running the app interactively, or use the following command to stop and remove the container:

```bash
docker-compose down
```

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.
