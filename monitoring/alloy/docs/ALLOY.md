# Grafana Alloy

Grafana Alloy collects host logs and forwards them according to `/etc/alloy/config.alloy`.

The template mounts the systemd journal read-only and joins `services.network` as `alloy`.

Origin validation: Passive Black Box documented Alloy 1.19.2 and successful systemd-journal delivery to Loki. Revalidate labels and destinations for the local deployment.
