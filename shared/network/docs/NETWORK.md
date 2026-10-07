# Shared services network

This Quadlet creates a private Podman bridge named `quadlet-services`.

Services in this library that need private container-to-container communication reference `services.network`. Podman DNS then allows containers to reach one another by `NetworkAlias` without publishing every application port on the host.

Copy `services.network` to `/etc/containers/systemd/` before activating services that reference it.

The network is intentionally not marked internal because monitoring, authentication, automation, certificate, and update workflows may need outbound access.

Origin validation: the equivalent network was validated on the Passive Black Box deployment with SELinux enforcing and survived full host reboot testing. This generic name and path layout must still be validated by each consuming system.
