# VictoriaMetrics

This template runs single-node VictoriaMetrics as a Prometheus-compatible metrics store.

Persistent state: `/var/lib/victoriametrics`.

The template joins `services.network` as `victoriametrics`.
