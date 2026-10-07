# NUT Exporter

NUT Exporter reads a local Network UPS Tools server and exposes selected UPS metrics to Prometheus.

The template expects NUT on `127.0.0.1:3493` and disables device-info metrics by default. Replace `@@NUT_EXPORTER_LISTEN_ADDRESS@@` before activation.

Origin validation: Passive Black Box documented NUT Exporter 3.3.0, local NUT connectivity, Prometheus and VictoriaMetrics queries, SELinux enforcing, and full reboot recovery. The old Passive-only dependency on its private monitoring network has intentionally been removed from this generic host-network template.
