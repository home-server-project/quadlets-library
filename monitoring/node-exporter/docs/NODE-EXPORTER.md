# Node Exporter

Node Exporter exposes host hardware and operating-system metrics.

The template follows the upstream container pattern with host networking, the host PID namespace, and the host root mounted read-only at `/host`. SELinux container labeling is disabled for that host-root mount.

Replace `@@NODE_EXPORTER_LISTEN_ADDRESS@@` before activation. Bind only to an address reachable by the intended Prometheus instance.

Origin validation: Passive Black Box documented Node Exporter 1.12.1, host filesystem and network metrics, SELinux enforcing, and full reboot recovery. The old Passive-only dependency on its private monitoring network has intentionally been removed from this generic host-network template.
