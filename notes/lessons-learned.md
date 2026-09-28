# Lessons learned

[Home](../README.md) · [Learning notes](../docs/learning.md) · [Experiments](experiments.md)

## Small hardware led to useful services

I started with a Raspberry Pi to understand what it could do. Discovering self-hosted services led me toward my own local storage setup. The Pi 5 now runs OMV with separate USB boot storage and an external data HDD.

## Modern resources are easy to take for granted

The Fujitsu's less than 1 GB RAM changed how I think about software resource use. An old Ubuntu release is installed, but the GUI issue remains. I want to understand the hardware support and required components before trying to simplify the system.

## Some history needs recovering

I do not remember why I first chose Void after working with Arch. The exact Ubuntu/kernel versions and sequence of Fujitsu attempts are also missing. For future experiments, I want to record the reason for a change alongside what happened.

## Keeping components creates another investigation

I kept usable parts from a disassembled old computer. Reusing them with a microcontroller will first require identifying their interfaces and electrical requirements.

## Local services raise wider questions

Operating storage brings permissions and recovery into the project. Pi-hole raises a different question: which parts of a lookup can I control locally, and who coordinates the systems beyond my network? That is the focus of the [planned DNS experiment](../experiments/dns-resolution-path.md).
