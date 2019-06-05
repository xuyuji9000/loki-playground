- Run promtail

``` bash
docker run -d \
-v $(pwd)/docker-config.yaml:/docker-config.yaml \
-v $(pwd)/log:/var/log \
grafana/promtail \
-config.file=/docker-config.yaml
```
