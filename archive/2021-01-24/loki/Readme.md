- Run loki

``` bash 
docker run -p 3100:3100 \
--restart=always \
-d \
-v $(pwd)/local-config.yaml:/local-config.yaml \
grafana/loki \
-config.file=/local-config.yaml
```
