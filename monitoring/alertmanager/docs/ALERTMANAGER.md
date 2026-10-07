# Alertmanager

Alertmanager receives alerts from Prometheus and routes notifications.

Configuration: `/etc/alertmanager/alertmanager.yml`.
Optional Telegram token: `/etc/alertmanager/secrets/telegram-bot-token`.
Persistent state: `/var/lib/alertmanager`.

The template joins `services.network` as `alertmanager`.
