# Authelia

Authelia provides authentication for selected self-hosted applications.

Environment file: `/etc/authelia/authelia.env`.
Configuration: `/etc/authelia/config/`.
Secrets: `/etc/authelia/secrets/`.
Persistent state: `/var/lib/authelia`.

The template joins `services.network` as `authelia` and also publishes `127.0.0.1:9091` for local host access.
