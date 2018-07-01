# Home Assistant configuration

Ensure all secrets are specified in `homeassistant/secrets.yaml`. List all
expected secrets:

```shell
awk '/!secret/{print $NF}' homeassistant/configuration.yaml
```

Start the Docker container with:

```shell
docker-compose up -d
```

The same command can be used to update to latest image after a `docker-compose
pull`.
