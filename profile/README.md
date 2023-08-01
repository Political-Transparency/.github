# Political Transparency - Installation Guide

# Client

## Introduction
This README file provides instructions on how to install and run your React app.

## Prerequisites
Make sure you have Docker installed on your system. <br>
You can download it from the official Docker website: https://www.docker.com/get-started

## Installation
<li> If you haven't already, clone or download your React app source code from the clinet repo.

<li> Build the Docker Image:<br>
Open a terminal or command prompt, navigate to the directory containing the Dockerfile, and run the following command to build the Docker image for your React app:

  ```
docker build -t my-react-app .
```
Replace my-react-app with a suitable name for your Docker image.

<li> Run the Docker Container:<br>
After building the Docker image, you can run your React app in a Docker container. Use the following command to start the container:

```
docker run -d -p 3000:3000 my-react-app
```
This command runs the container in detached mode (-d), maps port 3000 from the container to port 3000 on your host machine, and uses the image you built earlier (my-react-app).

<li> Access Your React App:<br>
Once the container is running, you can access your React app by opening a web browser and navigating to http://localhost:3000.
