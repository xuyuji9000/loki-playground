# loki-playground

- Run grafana: 

```bash 
docker run -d \
-p 3000:3000 \
grafana/grafana
```


- Install docker and docker-compose 

``` bash
yum install docker
sudo curl -L "https://github.com/docker/compose/releases/download/1.24.0/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
chmod +x /usr/local/bin/docker-compose
```