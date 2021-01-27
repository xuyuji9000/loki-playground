- Versions

    OS: **Centos 7**

    Loki: [v2.1.0](https://github.com/grafana/loki/tree/v2.1.0)

- Steps

0. Prepare working directory

    > `/srv/loki` used for Loki

1. Get Loki from [release page](https://github.com/grafana/loki/releases/)

    > Can use `curl -LO`[1] for this task

2. Unzip **.zip** file

3. Get base **Loki** configuration

    ``` bash
    # Pay attention to the version used here
    # Might need Wireguard VPN on for dowloading the configuration, considering the "https://raw.githubusercontent.com" connection within mainland China
    VERSION="v2.1.0"
    curl -LO https://raw.githubusercontent.com/grafana/loki/${VERSION}/cmd/loki/loki-local-config.yaml
    ```
4. Start

    ``` bash
    ./loki-linux-amd64 -config.file=loki-local-config.yaml
    ```

# Reference

1. [https://grafana.com/docs/loki/latest/installation/local/](https://grafana.com/docs/loki/latest/installation/local/)


2. [download-zip-file-with-curl-command](https://askubuntu.com/questions/285976/download-zip-file-with-curl-command#answer-291084)

    > Use `curl -LO` for downloading zip file
