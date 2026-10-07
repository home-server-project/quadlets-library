# VictoriaMetrics

This template runs single-node VictoriaMetrics as a Prometheus-compatible metrics store.

Persistent state: `/var/lib/victoriametrics`.
The template joins `services.network` as `victoriametrics`.

Origin validation: Passive Black Box documented VictoriaMetrics 1.151.0, successful Prometheus `up` queries, readiness checks, and full reboot recovery.
