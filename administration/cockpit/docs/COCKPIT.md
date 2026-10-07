# Cockpit web console

This template supplies the browser-facing Cockpit web service using `quay.io/cockpit/ws:latest`.

It mounts the host root and runs privileged with the host PID namespace because Cockpit is an administrative interface to the host. Review the trust boundary before exposing TCP 9090 and restrict access to intended management networks.

Origin validation: the source Passive Black Box deployment validated the Cockpit Quadlet on physical hardware, including administration pages, terminal access, automatic startup after reboot, and zero failed systemd units.
