# Caddy with Cloudflare DNS support

This is an optional Caddy template using `ghcr.io/highwaytoit/caddy-cloudflare-build:latest`.

It is not required by the library. Administrators can use their own Caddy image or another reverse proxy.

Environment file: `/etc/caddy/caddy.env`.
Caddyfile: `/etc/caddy/Caddyfile`.
Persistent data: `/var/lib/caddy/data` and `/var/lib/caddy/config`.

Replace `@@CADDY_BIND_ADDRESS@@` before activation. The supplied example keeps HTTPS on port 8443 to make the bind choice explicit.
