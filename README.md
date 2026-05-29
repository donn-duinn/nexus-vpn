# nexus-vpn

Custom mesh VPN — WireGuard + STUN + DERP relay + MagicDNS.

## Overview

Nexus VPN provides encrypted peer-to-peer mesh networking for the Tech Duinn cluster. It combines WireGuard for encryption, STUN for NAT traversal, DERP relay for fallback connectivity, and MagicDNS for human-readable node names.

## Features

- **WireGuard Mesh** — Full mesh encryption between all nodes
- **STUN NAT Traversal** — Direct peer connections without port forwarding
- **DERP Relay** — Fallback relay for restrictive networks
- **MagicDNS** — Human-readable hostnames for all nodes
- **Auto Key Rotation** — Periodic key refresh for forward secrecy
- **Health Monitoring** — Dashboard showing peer status and latency

## Nodes

| Node | Role | Address |
|------|------|---------|
| dagda | Master / GPU | dagda.tech-duinn.ts.net |
| brigid | Media Worker | brigid.tech-duinn.ts.net |
| cernunnos | Storage / DNS | cernunnos.tech-duinn.ts.net |
| aengus | Mobile | aengus.tech-duinn.ts.net |

## Tech Stack

- Go, WireGuard
- Tailscale (DERP infrastructure)
- STUN/TURN (via nexus-stun)

## License

MIT
