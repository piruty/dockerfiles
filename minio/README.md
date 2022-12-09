```bash
docker volume create minio
docker run -itd --name minio -p 9000:9000 -v minio:/data -e MINIO_ROOT_USER=admin -e MINIO_ROOT_PASSWORD=$MINIO_PASSWORD minio/minio server /data
```
