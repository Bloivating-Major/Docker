#### 1. Running Containers
```bash
docker run [OPTIONS] IMAGE [COMMAND]
```

Common Options:
- `-i` → Interactive mode (keeps STDIN open)
- `-t` → Allocate pseudo-TTY (terminal)
- `-it` → Combination for interactive terminal session
- `--name` → Assign a specific name to the container

Example:
```bash
docker run -it --name my_ubuntu ubuntu
```

#### 2. Container Lifecycle 🔄
- `docker start [CONTAINER]` → Start a stopped container
- `docker stop [CONTAINER]` → Stop a running container
- `docker restart [CONTAINER]` → Restart a container