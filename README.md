# loki

Working example of Loki, Promtail, and Grafana.

Promtail scrapes host system logs and Grafana logs. Then, you may query logs within the Grafana interface.

## getting started

```bash
$ alias dc=docker-compose
$ dc build
$ dc up -d && dc logs -f
$ open http://localhost:3000 # user/pass: admin
```

Configuration -> Data sources, Add Loki (http://loki:3100).

Explore -> Select 'Loki' from drop-down -> Click 'Log browser'.

## grafana shell

```bash
$ dc run --rm --entrypoint=/bin/sh grafana
```
