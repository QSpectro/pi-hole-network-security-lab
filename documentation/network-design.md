# Network Design

## Environment

- **DNS filtering host:** Raspberry Pi
- **Operating system:** Raspberry Pi OS
- **DNS filtering software:** Pi-hole
- **DNS configuration:** Home router configured to send DNS requests to Pi-hole
- **Administration method:** SSH / terminal
- **Network scope:** Personal home network

## DNS Request Flow

1. A client device makes a DNS request.
2. The home router directs DNS requests to the Pi-hole server, according to the configured network settings.
3. Pi-hole checks the request against its DNS filtering rules and cache.
4. If the request is allowed and requires external resolution, Pi-hole uses its configured upstream DNS resolver.
5. The response is returned to the requesting client.

## Verification

The following items will be verified and recorded:

- Raspberry Pi OS version
- Pi-hole service and blocking status
- Installed Pi-hole version
- Configured upstream DNS provider
- Successful DNS resolution
- DNS filtering behavior

## Security and Privacy

This documentation intentionally excludes credentials, public IP addresses, and sensitive network details.

No router configuration changes are required for the documentation process.

## Notes

The exact DNS forwarding behavior and upstream resolver will be documented after verification.
