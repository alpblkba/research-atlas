---
id: "provelengios-2019-power-distribution-attacks"
title: "Characterizing Power Distribution Attacks in Multi-User FPGA Environments"
authors: ["George Provelengios", "Daniel E. Holcomb", "Russell Tessier"]
year: 2019
venue: "FPL 2019, pp. 194-201"
doi: "10.1109/FPL.2019.00038"
source: "https://doi.org/10.1109/FPL.2019.00038"
status: "catalogued"
topics: ["physical-security", "dependable-computing"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Power distribution attacks in multi-user FPGAs

[Publication DOI](https://doi.org/10.1109/FPL.2019.00038) · [TRETS 2021 follow-up](https://doi.org/10.1145/3451236) · [Direction catalogue](index.md)

## Reading focus

This is the multi-tenant power-distribution study cited in my droop note. Read it against PWNN to separate the workload generating the load from the timing fault observed by its neighbor.

- Identifies mechanisms and possible mitigations, which helps separate the physical effect from the attack demonstration.
- A 2021 ACM TRETS follow-up proposes localized detection and clock suppression.

Reading tier: core for the multi-tenant FPGA thread.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: a tenant on a shared FPGA can use high-power circuits to disturb the supply voltage seen by another tenant and cause delay faults; the paper identifies the mechanisms and possible mitigations.

## Questions for the full paper

- On which FPGA family, and with which power-wasting structures, were the measurements made?
- How does the distance between attacker and victim regions affect the droop?
- Which mitigations are evaluated experimentally, and which are proposals?

## Connections

[Sensing nanosecond-scale voltage attacks in FPGAs](zick-2013-sensing-voltage-transients.md) · [PWNN: Power-Wasting Neural Network As Remote Fault Injector](xu-2026-pwnn.md) · [Active fences](krautter-2019-active-fences.md)
