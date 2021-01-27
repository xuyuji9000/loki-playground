- Versions

    OS: **Centos 7**

    Promtail: [v2.1.0](https://github.com/grafana/loki/tree/v2.1.0)

        > Promtail and Loki are distributed from the same link

- Steps

0. Prepare working directory

    > `/srv/promtail` used for Loki

    > `/srv`[1] maybe not optimal directory, but will use this for now.

1. Download 

    > Get from [release page](https://github.com/grafana/loki/releases/)

    > Searching keyword **promtail-linux-amd64**

2. Unzip

    > Unzip **.zip** file

3. Get base configuration

    ``` bash
    # Pay attention to the version used here
    # Might need Wireguard VPN on for dowloading the configuration, considering the "https://raw.githubusercontent.com" connection within mainland China
    VERSION="v2.1.0"
    curl -LO "https://raw.githubusercontent.com/grafana/loki/${VERSION}/cmd/promtail/promtail-local-config.yaml"
    ```

4. Start

# Reference

1. [Filesystem Hierarchy Standard](https://en.wikipedia.org/wiki/Filesystem_Hierarchy_Standard)
