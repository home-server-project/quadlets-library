# Grafana

Grafana provides dashboards and query access to observability data.

Environment file: `/etc/grafana/grafana.env`.
Persistent state: `/var/lib/grafana`.

The template joins `services.network` as `grafana` and publishes no host port.

Check ownership of the persistent data directory for the Grafana container user before activation.
