# Prometheus

Prometheus scrapes metrics and evaluates alert rules.

Configuration: `/etc/prometheus/prometheus.yml`.
Rules: `/etc/prometheus/rules/`.
Persistent state: `/var/lib/prometheus`.

The template joins `services.network` as `prometheus`.
