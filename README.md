Test Project

## Docker Image

The Docker image for this application is published to GitHub Container Registry (GHCR).

### Pull the image

```bash
docker pull ghcr.io/sneha-maria/nginx-devops-app:latest
```

### Run the container

```bash
docker run -d \
  --name nginx-devops-app \
  -p 8080:80 \
  ghcr.io/sneha-maria/nginx-devops-app:latest
```

### Access the application

Open the following URL in a web browser:

```text
http://localhost:8080
```

### Verify the container

```bash
docker ps
```

### Stop the container

```bash
docker stop nginx-devops-app
```

### Remove the container

```bash
docker rm nginx-devops-app
```

The application uses port 80 inside the container. Port 8080 on the host is mapped to the container's port 80.
git