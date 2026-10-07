# Blackbox Exporter

Blackbox Exporter performs active HTTP, TCP, ICMP, and DNS probes for Prometheus.

Configuration: `/etc/blackbox-exporter/blackbox.yml`.
The template joins `services.network` as `blackbox-exporter` and does not publish port 9115 on the host.

Origin validation: Passive Black Box documented Blackbox Exporter 0.28.0, HTTP/HTTPS, TCP, ICMP and DNS probes, Prometheus discovery, SELinux enforcing, and successful recovery after a full reboot.
