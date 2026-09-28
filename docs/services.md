# Services

[Home](../README.md) · [Architecture](architecture.md) · [Configuration notes](../configs/README.md)

## OpenMediaVault — active

OMV runs on my Raspberry Pi 5 with 8 GB RAM. The operating system boots from USB storage, and an external HDD holds data. My aim is a local personal-cloud environment for documents, photographs, and files used around the house.

I configured OMV with security in mind and consulted setup/documentation resources. Specific controls and observations belong in the [security notes](security.md).

### Still to document

OMV and underlying OS versions; HDD capacity, filesystem, shares, access permissions, encryption, redundancy, and backup/restore arrangements. These are not documented yet.

## Pi-hole — active

I use Pi-hole for DNS-level filtering. Host placement, version, upstream resolver, DHCP integration, local records, logging settings, and client coverage are not documented yet.

The next planned test is [From Pi-hole to the DNS Root](../experiments/dns-resolution-path.md), which compares resolution paths and a temporary local filtering rule.

## Networking — experimental

I am exploring OpenWrt, firewall rules, network security, and IoT isolation. The specific configuration changes and outcomes are not documented yet. See [networking](networking.md).

## Future services — planned

VPN remote access, network/security monitoring, automated backups, further self-hosted services, and services spread across multiple machines are on the [roadmap](roadmap.md). The [homelab-status design](../projects/homelab-status.md) describes a planned Rust tool for querying selected machine information.
