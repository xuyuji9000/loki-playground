- Run loki

``` bash 
docker run -p 3000:3000 \
-d \
-v $(pwd)/local-config.yaml:/local-config.yaml \
grafana/loki \
-config.file=/local-config.yaml
```
