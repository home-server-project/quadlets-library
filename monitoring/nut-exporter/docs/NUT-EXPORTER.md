# NUT Exporter

NUT Exporter reads a local Network UPS Tools server and exposes selected UPS metrics to Prometheus.

The template expects NUT on `127.0.0.1:3493` and disables device-info metrics by default.

Replace `@@NUT_EXPORTER_LISTEN_ADDRESS@@` before activation. Bind only to an address reachable by the intended Prometheus instance.
