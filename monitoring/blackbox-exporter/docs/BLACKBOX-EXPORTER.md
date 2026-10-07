# Blackbox Exporter

Blackbox Exporter performs active HTTP, TCP, ICMP, and DNS probes for Prometheus.

Configuration: `/etc/blackbox-exporter/blackbox.yml`.

The template joins `services.network` as `blackbox-exporter` and does not publish port 9115 on the host.
