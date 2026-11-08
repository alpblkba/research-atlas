---
id: "tang-2017-clkscrew"
title: "CLKSCREW: Exposing the Perils of Security-Oblivious Energy Management"
authors: ["Adrian Tang", "Simha Sethumadhavan", "Salvatore Stolfo"]
year: 2017
venue: "USENIX Security 2017, pp. 1057-1074"
doi: null
source: "https://www.usenix.org/conference/usenixsecurity17/technical-sessions/presentation/tang"
status: "catalogued"
topics: ["physical-security", "microarchitectural-security"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# CLKSCREW

[Source](https://www.usenix.org/conference/usenixsecurity17/technical-sessions/presentation/tang) · [Direction catalogue](index.md)

## Reading focus

In CLKSCREW a kernel driver controls voltage and frequency on a phone SoC. I want to trace the chain from that software interface to a physical timing failure.

- Targets Arm TrustZone, which connects physical faults to the trusted execution papers.

Reading tier: core.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the USENIX presentation page.

USENIX abstract: CLKSCREW abuses energy-management features to induce faults without physical access or fault-injection equipment; on commodity Arm/Android devices, a malicious kernel driver extracts keys from TrustZone and loads self-signed code into it.

## Questions for the full paper

- Which DVFS limits were missing in hardware, and could they be enforced without performance cost?
- How precise is the fault timing compared with on-FPGA ring-oscillator injection?
- Why is a kernel-privileged attacker still meaningful against TrustZone?

## Connections

[Plundervolt](murdock-2020-plundervolt.md) · [FPGAhammer](../../dependable-computing/papers/krautter-2018-fpgahammer.md) · [Keystone](../../microarchitectural-security/papers/lee-2020-keystone.md)
