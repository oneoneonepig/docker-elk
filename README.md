
## Create

```
touch /var/log/web/nginx.access.log
touch /var/log/web/nginx.error.log

docker-compose up -d
```

## Make some logs

```
./test.sh >/dev/null
```

# View

```
http://localhost:5601

curl http://localhost:9200/_cat/indices
```

## Delete

```
docker-compose down

rm /var/log/web/*

touch /var/log/web/nginx.access.log
touch /var/log/web/nginx.error.log
```
