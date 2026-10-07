# Loki

Loki stores logs and exposes them to Grafana.

Configuration: `/etc/loki/loki.yml`.
Persistent state: `/var/lib/loki`.
The template joins `services.network` as `loki`.

Origin validation: Passive Black Box documented Loki 3.7.7 receiving systemd-journal data from Alloy and surviving reboot testing.
