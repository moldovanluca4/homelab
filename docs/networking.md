# Networking

[Home](../README.md) · [Architecture](architecture.md) · [Security](security.md)

## Current work

The lab includes OMV on the Pi 5 and Pi-hole for DNS filtering. Router platform, DHCP provider, client DNS settings, and Pi-hole placement are not documented yet.

I am actively exploring OpenWrt, firewall rules, network security, and IoT isolation. OpenWrt's role in the network and specific tested rules are not documented yet. There are no recorded isolation-test results so far.

Dedicated trusted, IoT, guest, and experimental networks, VLANs, VPN access, monitoring, and traffic control remain planned.

## Reference notes

| Concept | Role in the lab |
| --- | --- |
| LAN | Connects local devices and services. |
| DHCP | Supplies network settings such as addresses, gateway, and DNS servers. |
| DNS | Resolves names and other records; Pi-hole handles filtering for clients that use it. |
| Routing | Forwards packets between networks. |
| Segmentation | Separates groups so access can be controlled. |
| VLANs | Provide logical separation at the link layer on compatible hardware. |
| Firewall zones | Group interfaces or networks under an access policy. |
| VPN | Provides an authenticated tunnel across another network. |

Routing and firewall rules determine communication between VLANs. OpenWrt distinguishes traffic to the router from traffic forwarded through it. See the [OpenWrt firewall documentation](https://openwrt.org/docs/guide-user/firewall/firewall_configuration).

## IoT isolation investigation

I want to establish which functions devices need, such as DNS and local control, before deciding which interactions to allow. Personally managed devices need appropriate access limits too.

The next practical step is to record the current setup and one proposed boundary, then compare expected and observed allowed/denied traffic with a rollback plan. This test is planned. Existing hardware's segmentation support also needs checking.

The [DNS resolution-path experiment](../experiments/dns-resolution-path.md) is the first concrete DNS test to perform. The [roadmap](roadmap.md) keeps the other network work in order.
