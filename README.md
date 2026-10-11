# Cloud-Based Web Application Deployment

## Project Overview

A Flask-based IT infrastructure dashboard packaged with Docker and prepared for deployment on AWS EC2 using Ubuntu Linux.

The dashboard provides a demonstration interface for viewing application services and deployment technologies.

## Technologies Used

- Python
- Flask
- HTML and CSS
- Docker
- Linux (Ubuntu)
- AWS EC2 (planned deployment)
- Git and GitHub
- Networking fundamentals (TCP/IP, ports, HTTP/HTTPS)

## Project Structure

```text
cloud-web-deployment/
├── app.py
├── requirements.txt
├── Dockerfile
├── .dockerignore
├── .gitignore
├── templates/
│   └── index.html
└── static/
    └── style.css
```

## Run Locally

1. Clone the repository:
   `git clone https://github.com/Ritansu2003/cloud-web-deployment.git`

2. Enter the project directory:
   `cd cloud-web-deployment`

3. Create and activate a Python virtual environment.

4. Install dependencies:
   `pip install -r requirements.txt`

5. Start the application:
   `python app.py`

6. Open `http://127.0.0.1:5000` in your browser.

## Run with Docker

Build the image:
`docker build -t cloud-web-dashboard:1.0 .`

Run the container:
`docker run -d --name cloud-web-dashboard -p 5000:5000 cloud-web-dashboard:1.0`

Open `http://127.0.0.1:5000`.

To view logs:
`docker logs cloud-web-dashboard`

To stop the container:
`docker stop cloud-web-dashboard`

## Current Status

- Flask dashboard built and tested locally.
- Docker image built successfully.
- Application running successfully inside a Docker container.
- AWS EC2 deployment: planned.

## Notes

Service statuses shown in the dashboard are demonstration values, not live infrastructure health checks.
