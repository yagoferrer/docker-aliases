# Docker Aliases

Docker Swarm

```bash
function dscheck() {
docker service ps --no-trunc "$1"
}
```

```bash
function dslogs() {
docker service logs "$1"
}
```

```bash
function dserrors() {
journalctl -u docker.service | tail -n 50 
}
```

