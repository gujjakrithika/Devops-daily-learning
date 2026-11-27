Today's Learning:

### Dockerfile
Learned how to create a Dockerfile, which is a set of instructions used to build a Docker image. A Dockerfile defines the application's environment, dependencies, files, and startup command.

## Key Instructions:
- FROM: Specifies the base image.
- WORKDIR: Sets the working directory inside the container.
- COPY: Copies files from host to container.
- RUN: Executes commands during image build.
- EXPOSE: Documents the port used by the application.
- CMD: Defines the default command when the container starts.

# Example:
FROM node:18
WORKDIR /app
COPY . .
RUN npm install
EXPOSE 3000
CMD ["npm", "start"]

Commands:
- docker build -t myapp .
- docker images


### Docker Images
Learned that a Docker image is a read-only template containing application code, runtime, libraries, and dependencies. Images are used to create containers.

Concepts:
- Images are built from Dockerfiles.
- Images are stored locally and can be pushed to registries such as Docker Hub.
- Containers are running instances of images.

Commands:
- docker images
- docker pull nginx
- docker rmi image_name
- docker inspect image_name


### Docker Volumes
Learned that volumes provide persistent storage for containers. Data stored in volumes remains available even if containers are stopped or deleted.

Benefits:
- Prevents data loss.
- Enables data sharing between containers.
- Separates application data from container lifecycle.

Commands:
- docker volume create myvolume
- docker volume ls
- docker volume inspect myvolume
- docker volume rm myvolume

Container with Volume:
docker run -v myvolume:/data nginx

Use Cases:
- Databases (MySQL, PostgreSQL)
- Application logs
- User uploads and persistent files


### Docker Compose
Learned how Docker Compose simplifies managing multi-container applications using a YAML configuration file (docker-compose.yml).

Benefits:
- Define infrastructure as code.
- Start multiple containers with a single command.
- Manage application dependencies easily.

Example:
version: "3"
services:
  web:
    image: nginx
    ports:
      - "80:80"

Common Commands:
- docker compose up
- docker compose up -d
- docker compose down
- docker compose ps
- docker compose logs
- docker compose restart


### Key Concepts Learned
- Dockerfile defines how an image is built.
- Docker image is a packaged application template.
- Docker container is a running instance of an image.
- Docker volumes provide persistent storage independent of containers.
- Docker Compose manages and orchestrates multiple containers from a single configuration file.
- Containers are lightweight, portable, and provide consistent environments across development, testing, and production.

### Common Docker Workflow
1. Write a Dockerfile.
2. Build an image using docker build.
3. Run a container from the image.
4. Mount volumes for persistent data if needed.
5. Use Docker Compose to manage multiple related containers.
