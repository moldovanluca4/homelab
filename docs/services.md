# Services

[Home](../README.md) · [Architecture](architecture.md) · [Configuration notes](../configs/README.md)

## In use — CURRENTLY IMPLEMENTED

| Service | Purpose | Details to add |
| --- | --- | --- |
| OpenMediaVault / NAS | Local storage | Host, version, disks, filesystem, capacity, shares, permissions, redundancy, encryption, backups |
| Pi-hole | DNS-level filtering | Host, version, upstream, client coverage, local records, DHCP integration |

I use OMV for the storage side of the project. Keeping private data and photos locally was one of the reasons I started self-hosting. The storage layout and recovery arrangements still need documenting.

Pi-hole is my DNS-filtering service. I need to record which clients use it and how their DNS settings are supplied. The [DNS notes](dns.md) cover resolution and filtering behavior.

## Experiments — EXPERIMENTAL

| Area | Purpose | Details to add |
| --- | --- | --- |
| Firewall rules | Explore device access policies | Platform, rules tried, and observations |
| IoT isolation | Explore separation of less trusted devices | Boundary mechanism and permitted traffic |
| OpenWrt | Explore networking and security configuration | Hardware, version, role, and features tried |

## Future services — PLANNED

| Area | Next decisions |
| --- | --- |
| VPN remote access | Protocol, endpoint, and access scope |
| Network/security monitoring | Tooling, retention, and alerts |
| Automated backups | Copy locations, retention, and restore procedure; existing manual arrangements TBD |
| Additional self-hosted/distributed services | Service selection, placement, and dependencies |
| Automation | Tasks worth automating and recovery steps |
| Arduino / smart-home integration | Hardware and project scope |

When a service changes, I will update this inventory and link the relevant [experiment notes](../notes/experiments.md). Installation, access checks, and restoration tests should have their own recorded outcomes.
