```bash
docker volume create portainer
docker run -d -p 9991:9000 --name=portainer --restart=always -v /var/run/docker.sock:/var/run/docker.sock -v portainer:/data portainer/portainer-ce:latest
```
