# Where local DNS control ends

[Home](../README.md) · [DNS notes](dns.md) · [Planned experiment](../experiments/dns-resolution-path.md)

I can control how names are resolved and filtered inside my home network, but who coordinates the system once the request depends on infrastructure outside my network?

Using Pi-hole made that question concrete. I can choose a local filtering rule. For a permitted lookup, the answer may depend on a recursive resolver and servers operated elsewhere.

## Following a lookup

Recursive resolvers obtain answers for clients. Root DNS, top-level domains, and delegations lead toward authoritative servers for a zone. Caches can shorten that process. The [DNS sequence diagram](dns.md) shows the roles.

The planned experiment compares local filtering with resolution through another path and an iterative trace. I want to distinguish a local policy decision from the information published by an authoritative server.

## Coordination and resilience

Domain names and IP addresses serve different purposes, but both depend on coordinated identifier systems. Shared protocols allow independently operated networks and software to communicate. I want to understand how DNS authentication, operational diversity, recovery, and dependencies affect resilience.

ICANN coordinates parts of the Internet's unique identifier systems, particularly DNS-related functions, within a wider ecosystem of operators, standards communities, registries, registrars, governments, and users. It does not control the Internet or its content. See [ICANN's explanation of its role](https://www.icann.org/resources/pages/what-2012-02-25-en).

The practical question from my lab leads to questions about how delegations are maintained, how changes are coordinated, and how technical requirements and governance decisions interact. The experiment can show lookup behavior; understanding institutional responsibilities also requires reading beyond its output.
