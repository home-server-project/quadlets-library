# Quadlets Library

Reusable Podman Quadlet templates for home servers and self-hosted systems.

## Purpose

This repository is a shared library of inactive Quadlet templates. The templates are intended to be easy to read, copy, customize, and maintain.

## Usage contract

- Templates in this repository do not start automatically.
- Copy the Quadlet you want into `/etc/containers/systemd/` and customize the local copy.
- Keep deployment-specific secrets, hostnames, addresses, and credentials outside this repository.
- Do not symlink a library template directly into the active Quadlet directory when the library is supplied by an OS image. A later image update could otherwise change an active service underneath the administrator.
- Generic templates use normal host locations such as `/etc/<service>/` for configuration and `/var/lib/<service>/` for persistent state. Change those paths when your storage layout requires it.
- `main` is the accepted library. No release or digest-resolution layer is required for normal consumption.

## Categories

- [Monitoring](./monitoring/) - metrics, logs, alerting, probes, exporters, and availability monitoring.
- [Administration](./administration/) - host administration interfaces.
- [Network & Access](./network-access/) - reverse proxy and authentication services.
- [Automation](./automation/) - workflow and diagnostic automation.
- [Shared](./shared/) - reusable Quadlet definitions shared by multiple services.

See [CATALOG.md](./CATALOG.md) for the complete service index.

## Service layout

A service directory can contain:

- the Quadlet template;
- `docs/` with deployment notes;
- `examples/` with safe example configuration.

The library favors simple copy-and-customize templates over a deployment framework. Any system with Podman Quadlet support can consume the templates independently.
