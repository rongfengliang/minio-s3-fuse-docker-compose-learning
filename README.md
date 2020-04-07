# minio + s3-fu docker-compose running

## How to Running


### 1. Start docker-composer (minio&&minio gateway)

```code
docker-compose up -d minio gateway
```

### 2. Create s3 bucket && upload some files

open http://localhost:9000 && upload some files

### 3. Start  s3-fs service

```code
docker-compose up -d app
```

### 4. View result

> inside container

```code
docker-compose exec app sh
ls /var/s3
```