# Git and Docker Starter Application

This repository contains a small Python web application used to practice Git, GitHub, and Docker workflows.

## Application

The application listens on port 8000 and returns a text response when accessed over HTTP.

## Verification

The running application should be verified using an HTTP request to port 8000.

## Usage

Build the image:

    docker build -t git-docker-app:test .

Run the container:

    docker run -d --name app-test -p 8080:8000 git-docker-app:test

Check the application:

    curl localhost:8080

Stop and remove the container:

    docker stop app-test
    docker rm app-test
