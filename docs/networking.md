# Networking

[Home](../README.md) · [Architecture](architecture.md) · [Security](security.md)

## Current work

The home network supports local services and Pi-hole. The router platform, DHCP provider, topology, and DNS client coverage still need documenting.

Firewall rules, IoT isolation, and OpenWrt are **EXPERIMENTAL**. I need to record the specific features tried and their results. OpenWrt's role in the network is TBD.

VLANs, dedicated trusted/IoT/guest networks, VPN access, monitoring, and traffic control are **PLANNED**.

## Reference notes

| Concept | Role | Detail to investigate in the lab |
| --- | --- | --- |
| LAN | Connects local devices. | Which devices share a network boundary? |
| DHCP | Supplies network settings such as addresses, gateway, and DNS servers. | Which system supplies those settings? |
| DNS | Resolves names and other records. | Which clients use Pi-hole? |
| Routing | Forwards packets between networks. | Which paths are needed between future segments? |
| Segmentation | Separates groups so access can be controlled. | Which interactions do IoT devices need? |
| VLANs | Provide logical separation at the link layer on compatible hardware. | What does the existing equipment support? |
| Firewall zones | Group interfaces or networks under a policy. | Which traffic reaches the router, and which passes through it? |
| VPN | Provides an authenticated tunnel across another network. | What should a remote client be able to reach? |

Routing and firewall rules determine communication between VLANs. In OpenWrt, traffic to the router is treated separately from traffic forwarded through it. See the [OpenWrt firewall documentation](https://openwrt.org/docs/guide-user/firewall/firewall_configuration).

## IoT isolation — EXPERIMENTAL

I want to separate personally managed devices from IoT, guest, and experimental devices. Current group membership, rules, and test results are TBD. A managed device can still be compromised, so required access matters within the trusted group too.

For the next isolation test, I need to identify necessary functions such as DNS and local control, then check allowed and denied traffic separately. Results will go in the [experiment log](../notes/experiments.md).

## Next steps — PLANNED

1. Record current DHCP, DNS, routing, and firewall roles.
2. Check the hardware's VLAN and segmentation support.
3. Test one boundary with expected traffic flows and a rollback plan.
4. Explore remote access, monitoring, and traffic control.
