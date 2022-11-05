# Docker

## Factorio Server

[Docker Hub Guide](https://hub.docker.com/r/factoriotools/factorio/)

Command to create: (Stored in `start_factorio.bash` on Gus):
```bash
sudo docker run -it \
    -p 34197:34197/udp \
    -p 27105:27105/tcp \
    -v /home/ubuntu/factorio:/factorio \
    --name factorio \
    --restart=always \
    factoriotools/factorio
```

Connect to console via:
```bash
docker attach factorio
```

Disconnect (detach) from container: <kbd>Ctrl</kbd>+<kbd>P</kbd>,<kbd>Ctrl</kbd>+<kbd>Q</kbd>