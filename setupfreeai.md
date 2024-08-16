# FreeGPT-WebUI-v2 Setup Guide

## Prerequisites
Before you start, make sure you have installed Docker on your machine.

## Running the Docker

### Dockerfile for Creating a Docker Image Yourself
You can create an image using the following commands:

```bash
git clone https://github.com/VadimBoev/freegpt-webui-v2.git
cd freegpt-webui-v2
```
# Update the requirements.txt File:
If the project has a requirements.txt file, make sure flask_babel is listed in it. This ensures that all necessary dependencies are installed when the container is built or run.

### Build Image:

```bash
docker build -f Dockerfile -t freegpt-webui-v2 .
```

### Run the Application Using Docker:

```bash
docker run -p 1338:1338 freegpt-webui-v2:latest
```

### Access the Application
You can access the application in your browser using the URL:

- [http://127.0.0.1:1338](http://127.0.0.1:1338)
- [http://localhost:1338](http://localhost:1338)

### Stop the Docker Containers
When you're done using the application, stop the Docker containers using the following command:

```bash
docker stop <container-id>
docker system prune -a

```

https://github.com/ChatTeach/FreeGPT-4?tab=readme-ov-file#api-g4f
