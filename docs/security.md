# Security

[Home](../README.md) · [Networking](networking.md)

I want to protect household data and limit unnecessary access between devices. Running the storage myself means deciding how to manage access, updates, and recovery.

## Currently configured

OMV runs on the Raspberry Pi 5 with USB boot storage and an external data HDD. I consulted setup/documentation resources, but the specific access controls, update arrangements, and checks are not documented yet.

Pi-hole is in use for DNS-level filtering. Its client coverage and resolver settings are not documented yet. DNS filtering acts on names; clients using another DNS path may bypass it, and it does not inspect all traffic.

## Currently being investigated

OpenWrt, firewall rules, network security, and IoT isolation are active areas of exploration. Specific rules and observed outcomes are not documented yet.

For the NAS, I want to record which accounts can access shares and administration, and how permissions match those roles. For the network, I want to establish what is externally reachable and distinguish router input from traffic forwarded between devices. Least privilege applies to managed devices as well as IoT devices.

## Planned work

- Document software versions and update/maintenance arrangements.
- Record current port forwarding and remote administration before changing exposure.
- Test a network boundary against expected allowed and denied traffic.
- Document existing backups and perform a restoration test with disposable test data.
- Define the access scope for a future VPN.
- Choose useful monitoring data, retention, and alerts.

The boot device and data HDD are separate storage roles, not a documented backup strategy. Backup copies, retention, redundancy, encryption, and restoration results are not documented yet. Backup automation remains planned.

## DNS and privacy

DNS logs can reveal device and family browsing activity. The [planned DNS experiment](../experiments/dns-resolution-path.md) uses a reserved example domain and restores the previous filtering state after testing. Its results will apply to the tested client and resolver paths.

For each change, record the starting state, expected behavior, observations, and rollback steps in the [experiment log](../notes/experiments.md).
