#### 3. Image Management 📦
- `docker pull [IMAGE]` → Download an image
- `docker push [IMAGE]` → Upload an image to registry
- `docker rmi [IMAGE]` → Remove an image


## Common Usage Patterns 🎯

### 1. Interactive Shell Session
```bash
# Start new Ubuntu container with interactive shell
docker run -it ubuntu bash

# Connect to running container
docker exec -it container_name bash
```

### 2. Container Management
```bash
# Run container with custom name
docker run -it --name my_container ubuntu

# List all containers
docker ps -a

# Remove container
docker rm container_name
```