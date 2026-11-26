# DOCKER

## Docker installieren (Ubuntu/Debian, offizielles Repository)
```bash
sudo apt install -y docker.io
sudo apt install -y docker-compose
```

## Installation prüfen
```bash
docker --version
docker compose version
docker run hello-world
```

## Stop immediately
```bash
systemctl stop docker
```

## Disable autostart on boot (stays off after reboot)
```bash
systemctl disable docker
```

## Start manually when needed
```bash
systemctl start docker
```

## Re-enable autostart on boot
```bash
systemctl enable docker
```

## Check status
```bash
systemctl status docker
```
```bash
systemctl is-enabled docker
```
```bash
systemctl is-active docker
```

## Docker über service-Befehl steuern (Alternative zu systemctl)
```bash
sudo service docker start
sudo service docker stop
sudo service docker restart
sudo service docker status
```

## Update Docker
```bash
sudo apt-get update
sudo apt-get install --only-upgrade -y docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
```

## List all Docker containers
```bash
docker ps -a
```

## List all Docker images
```bash
docker images
```

## Start containers with Compose
```bash
docker compose up -d
docker compose up -d --build
```

## Stop containers with Compose
```bash
docker compose down
```

## Delete containers/images (frees up disk space)
#### Container löschen
```bash
docker rm container_id
```
#### Image löschen
```bash
docker rmi image_id
```
#### Alles Ungenutzte aufräumen (Container, Netzwerke, Images, Cache)
```bash
docker system prune -a
```

## Container stoppen (läuft weiter im Hintergrund erhalten, nicht gelöscht)
```bash
docker stop container_id
```
