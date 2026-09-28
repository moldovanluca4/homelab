# Security

[Home](../README.md) · [Networking](networking.md)

I want to protect private data and reduce unnecessary access between devices, including those used by my family. Pi-hole is in use; firewall rules and IoT isolation are experimental. Stronger segmentation, monitoring, VPN access, and backup automation are planned.

## Access control and storage

My goal is to give devices and accounts the access they need for their role. For OMV, I still need to document share permissions, administrative access, software maintenance, encryption, and recovery arrangements.

Personally managed devices also need access limits. Trust should reflect a device's purpose and management rather than give it unrestricted administrative permissions.

## Network boundaries

I am exploring firewall rules and IoT isolation. The current rules, boundaries, and observed allowed/denied traffic are TBD. Router input and traffic forwarded between networks need separate attention.

I want local administration and storage to be reachable only where needed. Port forwarding, remote administration, and current inbound exposure still need checking and documenting.

## DNS filtering

Pi-hole provides name-based filtering. Client coverage and alternative DNS paths need checking. The [DNS notes](dns.md) explain how queries can be answered locally, blocked, or forwarded upstream.

## Backups — improvements PLANNED

A NAS or redundant disks alone do not provide a separate recoverable backup. I need to document existing copies, access, retention, and restoration results. Automated backups are planned; current manual arrangements are TBD.

## VPN and monitoring — PLANNED

For remote access, I want to define which services a VPN client should reach before choosing a configuration. For monitoring, I need to decide what to collect, how long to keep it, and which events need attention. DNS and network logs can expose family browsing and device activity, so collection should be limited to the operational questions being investigated.

## Recording changes

For each security experiment, I want to record the starting configuration, expected behavior, actual observations, and rollback steps. Those notes will help me revisit rules as devices and services change.
