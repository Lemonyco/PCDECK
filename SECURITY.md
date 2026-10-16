# Security

PCDeck is a local-network remote-control product. Security is treated as a product feature.

## Design principles
- Pairing and trusted-device sessions are required for control endpoints.
- Tablet clients use bounded action IDs instead of arbitrary executable paths.
- PCDeck intentionally does not expose a generic remote shell.
- Host/origin validation and rate limiting protect local HTTP surfaces.
- Workspace and LiveDeck restore operations use server-owned IDs and bounded window actions.
- Firewall rules should be scoped to the PCDeck executable and local subnet where possible.

## Reporting a vulnerability
Do not open a public issue for a security vulnerability. Use GitHub private vulnerability reporting once enabled, or contact the project owner privately.
