# SNMP Exporter

SNMP Exporter polls SNMP-capable devices and exposes the results as Prometheus metrics.

Environment file: `/etc/snmp-exporter/snmp.env`.
Additional auth configuration: `/etc/snmp-exporter/snmp-auth.yml`.
The template joins `services.network` as `snmp-exporter` and does not publish port 9116 on the host.

Origin validation: Passive Black Box documented SNMP Exporter 0.30.1 against MikroTik RouterOS, Prometheus service discovery, SNMPv3 auth expansion, and full reboot recovery.
