# Loki

Loki stores logs and exposes them to Grafana.

Configuration: `/etc/loki/loki.yml`.
Persistent state: `/var/lib/loki`.

The template joins `services.network` as `loki`.
