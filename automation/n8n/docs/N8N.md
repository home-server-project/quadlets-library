# n8n

n8n provides workflow automation.

Environment file: `/etc/n8n/n8n.env`.
Persistent state: `/var/lib/n8n`.

The template joins `services.network` as `n8n`, publishes no host port, drops all Linux capabilities, enables no-new-privileges, and uses a local health check.

Keep the live n8n SQLite database on local storage rather than NFS or another network filesystem.
