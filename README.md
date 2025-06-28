# Lakehouse
The Iceberg Lakehouse playground

## Setup
In your terminal, first type:

```
docker compose build spark
```

This builds up the image required for the Spark service including a Jupyter Notebook for development.


Next, type:
```
docker compose up -d
```
To spin up all services.

You'll need your IP address to have your blob storage. So run
```
docker inspect minio
```
and save the IP Address to a .env file.

To spin down all services:
```
docker compose down -v
```