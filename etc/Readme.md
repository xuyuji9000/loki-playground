- Install grafana: `sudo yum install grafana`

- Enable grafana starting from server boot:

    ``` bash
    systemctl enable grafana-server
    systemctl start grafana-server
    ```
- Check service running: `curl localhost:3000`
