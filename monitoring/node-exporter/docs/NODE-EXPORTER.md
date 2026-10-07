# Node Exporter

Node Exporter exposes host hardware and operating-system metrics.

The template uses host networking, the host PID namespace, and the host root mounted read-only at `/host`. SELinux container labeling is disabled for that host-root mount.

Replace `@@NODE_EXPORTER_LISTEN_ADDRESS@@` before activation. Bind only to an address reachable by the intended Prometheus instance.
