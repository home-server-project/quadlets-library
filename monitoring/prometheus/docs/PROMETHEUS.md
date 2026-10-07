# Prometheus

Prometheus scrapes metrics and evaluates alert rules.

Configuration: `/etc/prometheus/prometheus.yml`.
Rules: `/etc/prometheus/rules/`.
Persistent state: `/var/lib/prometheus`.
The template joins `services.network` as `prometheus`.

Origin validation: Passive Black Box documented Prometheus 3.14.0, Alertmanager delivery, remote write to VictoriaMetrics, and successful full-host reboot recovery.
