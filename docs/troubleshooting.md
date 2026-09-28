# Fujitsu laptop: older Ubuntu and an unresolved GUI problem

[Home](../README.md) · [Hardware](hardware.md) · [Experiment index](../notes/experiments.md)

**Status: Ongoing investigation.**

## Context

This Fujitsu laptop has been in my family for approximately 10–15 years. I wanted to see what I could still run on it, but modern and lightweight operating systems were difficult to use on the machine.

## Hardware constraints

- Memory: **less than 1 GB RAM**.
- **CPU model not yet verified; believed to be Pentium 4-class.**
- Exact model, graphics hardware, and storage: not documented yet.

## Initial problem

The laptop has very limited resources and compatibility problems. Even distributions intended for older hardware were difficult to run properly. The exact failure symptoms and distribution versions from those attempts are not documented yet.

## What I tried

I eventually installed an old Ubuntu release. Its exact release and kernel version are currently unknown. Installation got me to a system with a remaining graphical/GUI problem, so the investigation is still ongoing.

I also began researching older kernels and kernel/hardware compatibility. A version-by-version record of those attempts is not documented yet.

## Why I started looking at kernels

I want to understand which kernel components and modules this hardware actually needs, and how much could be removed or simplified on such a constrained machine. That is a direction for the next investigation; module or library removal has not been carried out in the recorded work.

The graphical problem could involve several layers. The hardware, driver, kernel, display server, and desktop/session behavior need distinguishing before I can narrow down a cause.

## Current unresolved GUI issue

A graphical problem remains after installing Ubuntu. Its exact behavior, error messages, and conditions are not documented yet. The first step is to describe what appears on screen and when the problem starts, rather than assume that a kernel change will solve it.

## What I learned

Using a machine with less than 1 GB RAM made me notice how accustomed I am to modern computers with abundant memory and CPU resources. I became more interested in resource-conscious software, operating systems, and the constraints older programmers worked within.

The investigation also connects to my growing interest in low-level systems and vulnerability/security research. For now, the practical problem is understanding this machine's hardware support and unresolved GUI behavior.

## Information still to recover

The exact laptop and CPU models, graphics hardware, installed Ubuntu release/kernel, earlier distributions tried, original symptoms, research sources, and the sequence of changes are not documented yet. Dates are also missing.

## Next investigation — planned

1. Identify the hardware and installed software versions without changing the installation.
2. Record the GUI symptom, relevant errors, and whether a text console works.
3. Separate possible resource limits from graphics-driver, display-server, and session problems.
4. Compare the findings with kernel/hardware support information and choose one change to test.
5. Keep a recoverable starting point and record each change and outcome.
6. Investigate required modules and possible simplification after identifying the baseline.

Before assigning the laptop a network service role, check the installed software's maintenance status and exposure.
