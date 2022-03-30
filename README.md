# loki

Scrapes host system logs and Grafana logs. Query logs within Grafana

## getting started

```bash
$ alias dc=docker-compose
$ dc pull
$ dc build
$ dc up -d && dc logs -f
$ open http://localhost:3000 # user/pass: admin
```

Configuration -> Data sources, Add Loki (http://loki:3100).

Explore -> Log browser

## grafana shell

```bash
$ dc run --rm --entrypoint=/bin/sh grafana
```
