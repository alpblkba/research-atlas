---
id: "amar-2023-cheriot"
title: "CHERIoT: Complete Memory Safety for Embedded Devices"
authors: ["Saar Amar", "David Chisnall", "Tony Chen", "Nathaniel Wesley Filardo", "Ben Laurie", "Kunyan Liu", "Robert Norton", "Simon W. Moore", "Yucong Tao", "Robert N. M. Watson", "Hongyan Xia"]
year: 2023
venue: "MICRO 2023, pp. 641-653"
doi: "10.1145/3613424.3614266"
source: "https://doi.org/10.1145/3613424.3614266"
status: "catalogued"
topics: ["microarchitectural-security", "operating-systems", "computer-architecture"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# CHERIoT

[Publication DOI](https://doi.org/10.1145/3613424.3614266) · [Direction catalogue](index.md)

## Reading focus

This entry is based on a truncated abstract. Check the full paper before relying on the technical description below.

CHERIoT brings capabilities to a microcontroller-class RISC-V core. That gives me an embedded setting in which to compare fine-grained authority with the protection boundaries I already work with.

- Designs memory safety and compartmentalization together with a small RTOS, hardware/OS co-design at embedded scale.
- The CHERIoT RTOS paper (SOSP 2025) continues the line on the OS side.

Reading tier: core for embedded security.

## Source record

Source check by agent, 2026-11-06: metadata from OpenAlex; the abstract in the record is truncated.

OpenAlex abstract (truncated in the record after the motivation): embedded devices need strong isolation and memory safety without the power, cost, scalability or real-time penalties of existing approaches.

## Questions for the full paper

- Which capability features are kept and which are dropped relative to full CHERI?
- How are heap temporal safety and revocation handled on a microcontroller?
- What does the core cost in area and cycles compared with a non-CHERI equivalent?

## Connections

[Thunderclap](../../operating-systems/papers/markettos-2019-thunderclap.md) · [Keystone](lee-2020-keystone.md) · [ISA semantics in Sail](../../computer-architecture/papers/armstrong-2019-isa-semantics-sail.md)
