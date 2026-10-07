# OpenClaw

This template provides a request-driven OpenClaw gateway intended for controlled automation or diagnostic workflows.

Environment file: `/etc/openclaw/openclaw.env`.
Application state: `/var/lib/openclaw`.
Provider authentication state: `/var/lib/openclaw-auth`.

The baseline drops all Linux capabilities, enables no-new-privileges, publishes no host port, and joins `services.network` as `openclaw`.

The example configuration intentionally disables elevated tools, browser control, autonomous workshop activity, heartbeat activity, and unrestricted Telegram access.
