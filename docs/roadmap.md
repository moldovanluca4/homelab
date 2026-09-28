# Roadmap

[Home](../README.md) · [Service inventory](services.md) · [Experiment log](../notes/experiments.md)

## In use — CURRENTLY IMPLEMENTED

- [x] Raspberry Pi hardware and Linux.
- [x] OMV for NAS/local storage.
- [x] Pi-hole for DNS filtering.

Old-laptop compatibility, firewall rules, IoT isolation, and OpenWrt are **EXPERIMENTAL**. I still need to record their exact scope and outcomes.

All unchecked items below are **PLANNED**, including the next steps for existing experiments.

## Short term

- [ ] Fill in the hardware inventory and service-to-device mapping.
- [ ] Record current network roles, firewall rules, and IoT-isolation scope.
- [ ] List the OpenWrt features tried and their outcomes.
- [ ] Document storage, existing backups, and a restoration-test plan.
- [ ] Record Pi-hole client coverage and upstream behavior.
- [ ] Fill in the laptop/kernel investigation, including unresolved failures.

## Medium term

- [ ] Continue OpenWrt experiments with observations and rollback notes.
- [ ] Explore VLANs and dedicated trusted, IoT, guest, and experimental networks.
- [ ] Develop firewall policies around required traffic.
- [ ] Explore VPN remote access with a defined access scope.
- [ ] Add network/security monitoring and decide on log retention.
- [ ] Improve backups, test restoration, and explore backup automation.
- [ ] Experiment with local DNS, recursion, caching, and DNS security.
- [ ] Explore traffic control and assess whether it helps with a specific need.

## Long term

- [ ] Automate repeated administration tasks with recovery steps.
- [ ] Add self-hosted services and document their dependencies.
- [ ] Distribute services across machines and observe failure behavior.
- [ ] Study Internet identifiers, standards, coordination, and resilience.
- [ ] Revisit access policies as devices and services change.

## Creative ideas — PLANNED

- [ ] Explore Arduino integration and smart-home projects.
- [ ] Repurpose more legacy hardware.
- [ ] Investigate reusing an old DVD player's screen; feasibility TBD.
- [ ] Keep notes on abandoned approaches and unexpected results.

When I begin an investigation, its status becomes EXPERIMENTAL. When a service goes into use, its status becomes CURRENTLY IMPLEMENTED. I will link dated observations separately and update the service inventory and diagrams alongside the change.
