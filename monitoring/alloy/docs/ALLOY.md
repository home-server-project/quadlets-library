# Grafana Alloy

Grafana Alloy collects host logs and forwards them according to `/etc/alloy/config.alloy`.

The template mounts the systemd journal read-only and joins `services.network` as `alloy`.
