# Home Server Quadlets Library

Reusable Podman Quadlet templates maintained by the Home Server Project.

## Purpose

This repository is a shared library of inactive Quadlet templates for home servers and small self-hosted systems. The templates are intended to be easy to read, copy, customize, and maintain.

The initial library was generalized from Quadlets validated in the Passive Black Box project. Product-specific names and paths are removed here, while useful validation notes are kept in the service documentation.

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
- `docs/` with deployment and validation notes;
- `examples/` with safe example configuration.

The library favors simple copy-and-customize templates over a deployment framework. Operating-system projects such as Rose and Gina can embed the complete library as inactive templates and let the local administrator choose what to activate.

## Validation

Validation notes describe what was tested on the original deployment and are not a promise that every template has been tested on every distribution, network, or storage layout. Revalidate the local copy after changing paths, network exposure, privileges, or application configuration.
