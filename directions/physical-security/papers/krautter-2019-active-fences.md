---
id: "krautter-2019-active-fences"
title: "Active Fences against Voltage-based Side Channels in Multi-Tenant FPGAs"
authors: ["Jonas Krautter", "Dennis R. E. Gnad", "Falk Schellenberg", "Amir Moradi", "Mehdi B. Tahoori"]
year: 2019
venue: "ICCAD 2019, pp. 1-8"
doi: "10.1109/ICCAD45719.2019.8942094"
source: "https://doi.org/10.1109/ICCAD45719.2019.8942094"
status: "catalogued"
topics: ["physical-security"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Active fences

[Publication DOI](https://doi.org/10.1109/ICCAD45719.2019.8942094) · [Direction catalogue](index.md)

## Reading focus

My voltage-droop note cites active fences. In this paper the ring oscillators supply defensive noise between a sensor and a victim, a different role from the aggressor grid in tasks 4 and 5.

- From the KIT CDNC group, complementing FPGAhammer and An Inside Job, which are already in the vault.

Reading tier: core for the multi-tenant FPGA thread.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: ring-oscillator active fences placed between an attacker circuit and a victim core reduce leakage on a Lattice ECP5 FPGA; against an AES-128 module, attackers needed about two orders of magnitude more traces, with no change to the protected module.

## Questions for the full paper

- How much power does the fence draw, and does it create its own fault risk?
- Does the fence remain effective against sensors placed closer to the victim?
- Would the result transfer to the iCE40 devices used in the hardware-security tasks?

## Connections

[An Inside Job](../../dependable-computing/papers/schellenberg-2018-inside-job.md) · [FPGAhammer](../../dependable-computing/papers/krautter-2018-fpgahammer.md) · [Sensing nanosecond-scale voltage attacks in FPGAs](zick-2013-sensing-voltage-transients.md)
