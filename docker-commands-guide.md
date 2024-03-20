# Docker Commands Guide

## Docker Container Management

- `docker ps`: List running containers
- `docker ps -a`: List all containers (including stopped ones)
- `docker start <container_id>`: Start a stopped container
- `docker stop <container_id>`: Stop a running container
- `docker restart <container_id>`: Restart a running container
- `docker rm <container_id>`: Remove a stopped container
- `docker rm -f <container_id>`: Forcefully remove a running container

## Docker Image Management

- `docker images`: List all images
- `docker pull <image_name>`: Pull an image from Docker Hub
- `docker build -t <image_name> .`: Build an image from a Dockerfile in the current directory
- `docker tag <image_id> <new_image_name>`: Tag an image with a new name
- `docker rmi <image_id>`: Remove an image

## Docker Network Management

- `docker network ls`: List all networks
- `docker network inspect <network_name>`: Inspect a network
- `docker network create <network_name>`: Create a new network
- `docker network connect <network_name> <container_name>`: Connect a container to a network
- `docker network disconnect <network_name> <container_name>`: Disconnect a container from a network

## Docker Volume Management

- `docker volume ls`: List all volumes
- `docker volume inspect <volume_name>`: Inspect a volume
- `docker volume create <volume_name>`: Create a new volume
- `docker volume rm <volume_name>`: Remove a volume
