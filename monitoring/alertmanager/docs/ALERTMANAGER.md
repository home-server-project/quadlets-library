# Alertmanager

Alertmanager receives alerts from Prometheus and routes notifications.

Configuration: `/etc/alertmanager/alertmanager.yml`.
Optional Telegram token: `/etc/alertmanager/secrets/telegram-bot-token`.
Persistent state: `/var/lib/alertmanager`.

The template joins `services.network` as `alertmanager`.

Origin validation: Passive Black Box documented Alertmanager 0.34.0, Prometheus alert delivery, Telegram firing/resolved notifications, readiness checks, and recovery after a full host reboot.
