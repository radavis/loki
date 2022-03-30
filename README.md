# loki

Working example of Loki, Promtail, and Grafana.

Promtail scrapes host system logs and Grafana logs. Then, query logs within Grafana interface.

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
