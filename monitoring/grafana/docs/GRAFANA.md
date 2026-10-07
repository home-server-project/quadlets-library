# Grafana

Grafana provides dashboards and query access to observability data.

Environment file: `/etc/grafana/grafana.env`.
Persistent state: `/var/lib/grafana`.
The template joins `services.network` as `grafana` and publishes no host port.

Origin validation: the source Passive Black Box deployment used this pattern behind Caddy with Authelia/OIDC and validated persistence after reboot. Revalidate ownership for the local Grafana UID/GID before activation.
