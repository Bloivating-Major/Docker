## Quick Reference Card 📋

```ascii
+-------------------------+
|    Container Ops 🔄     |
+-------------------------+
run   → Create & start
start → Start existing
stop  → Stop running
rm    → Remove container

+-------------------------+
|    Image Ops 📦         |
+-------------------------+
pull  → Download image
push  → Upload image
rmi   → Remove image
images→ List images
```

## Best Practices 💡

1. Always name your containers
   ```bash
   docker run --name meaningful_name image_name
   ```

2. Clean up unused containers
   ```bash
   docker rm $(docker ps -aq)
   ```

3. Use appropriate flags
   - `-d` for detached mode
   - `-p` for port mapping
   - `-v` for volume mounting

## Common Issues and Solutions 🔧

### 1. Container Access
Problem: Cannot access container shell
Solution: Use `docker exec -it container_name bash`

### 2. Port Conflicts
Problem: Port already in use
Solution: Use different port mapping with `-p`

## Practice Exercises 💻

1. Basic Container Management
   ```bash
   # Create and run Ubuntu container
   docker run -it --name practice_ubuntu ubuntu
   
   # List running containers
   docker ps
   
   # Stop and remove container
   docker stop practice_ubuntu
   docker rm practice_ubuntu
   ```

2. Image Management
   ```bash
   # Pull specific image version
   docker pull ubuntu:20.04
   
   # List downloaded images
   docker images
   ```

## Next Steps 🚀

- Learn about Docker volumes
- Explore Docker networking
- Understand Docker Compose
- Practice building custom images

Ready to try these commands? Start with basic container operations and gradually move to more complex scenarios! 🎉