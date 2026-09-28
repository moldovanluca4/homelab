# From local DNS to Internet infrastructure

[Home](../README.md) · [DNS notes](dns.md)

Working with Pi-hole made me want to understand what happens beyond my local DNS settings. Inside the home network, I can choose local services, firewall rules, and access policies. Outside it, my devices rely on systems run by other people and organizations.

## DNS and identifiers

DNS has a distributed hierarchy. Recursive resolvers obtain answers, root servers help locate top-level-domain servers, and delegations lead to authoritative servers for particular zones. Caching reduces repeated lookups. The [DNS sequence diagram](dns.md) shows that process; [Cloudflare's explanation](https://www.cloudflare.com/learning/dns/what-is-dns/) provides more background.

Domain names and IP addresses have different roles, and both rely on coordination to remain useful globally. I want to understand how a name lookup fits into that wider system of Internet identifiers.

## Standards and resilience

The Internet joins independently operated networks and software implementations. Shared protocols let those systems communicate.

I want to study how DNS authentication, operational diversity, and recovery practices affect resilience, and how failures can spread through dependencies. These are future reading and experiment topics.

## Coordination and ICANN

ICANN coordinates parts of the Internet's unique identifier systems, particularly DNS-related functions. It works within a wider ecosystem of operators, standards communities, registries, registrars, governments, and users. ICANN does not control the Internet or its content. See [ICANN's explanation of its role](https://www.icann.org/resources/pages/what-2012-02-25-en).

Questions I want to follow up on:

- How are changes to shared naming infrastructure coordinated?
- How do technical requirements influence governance decisions?
- Whose operational needs are considered when those decisions are made?
- How do independently operated systems preserve interoperability?

These questions grew out of using DNS at home. I want to keep studying them alongside Linux, networking, systems programming, and distributed systems.
