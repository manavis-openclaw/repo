# Access and Network

## Access Paths
- Primary access method: SSH
- SSH host: x162-43-52-68 (public IP observed in OpenClaw status: 162.43.52.68)
- SSH port: 22
- SSH user: root
- Authentication method: manual input needed
- Emergency access path: provider web console or rescue mode, if available
- VPN / tailnet details: Tailscale is off at capture time

## Public Entry Points
- Public IP or hostname: 162.43.52.68
- Domain names in use: manual input needed
- Reverse proxy or tunnel: none confirmed
- Exposed services: SSH on 22, OpenClaw bound to loopback only on 18789 and 18791

## DNS
- DNS provider: manual input needed
- Zones managed: manual input needed
- Important records:
  - Name: manual input needed
    Type: manual input needed
    Target: manual input needed
    Notes: add only non-secret routing details here

## Firewall / Ports
- Firewall tool: no UFW status output captured, manual confirmation needed
- Allowed inbound ports: 22 confirmed, others not confirmed as public
- Allowed management sources: manual input needed
- Notes: OpenClaw control surface appears loopback-only. If exposed later through a reverse proxy, trusted proxy settings should be recorded.
