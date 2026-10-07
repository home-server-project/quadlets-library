# Uptime Kuma

Uptime Kuma provides simple service and device availability monitoring.

Persistent state: `/var/lib/uptime-kuma`.
The template joins `services.network` as `uptime-kuma`, publishes no host port, and grants only `CAP_NET_RAW` for probe support.

Keep the live database on local storage rather than NFS or another network filesystem.

Origin validation: Passive Black Box documented SELinux enforcing, reverse-proxy access, monitor recovery, and automatic service recovery after a full host reboot.
