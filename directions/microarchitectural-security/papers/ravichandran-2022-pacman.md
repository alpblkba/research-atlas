---
id: "ravichandran-2022-pacman"
title: "PACMAN: Attacking ARM Pointer Authentication with Speculative Execution"
authors: ["Joseph Ravichandran", "Weon Taek Na", "Jay Lang", "Mengjia Yan"]
year: 2022
venue: "ISCA 2022, pp. 685-698"
doi: "10.1145/3470496.3527429"
source: "https://doi.org/10.1145/3470496.3527429"
status: "catalogued"
topics: ["microarchitectural-security"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# PACMAN

[Publication DOI](https://doi.org/10.1145/3470496.3527429) · [Direction catalogue](index.md)

## Reading focus

PACMAN pairs a memory-safety bug with speculative pointer authentication on the M1. I want to separate the access the bug already grants from the information the speculative check reveals.

- One of the main papers that reverse-engineer Apple Silicon microarchitecture for security analysis.

Reading tier: core for the Apple Silicon thread.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: memory corruption and speculative execution can be combined to bypass Arm Pointer Authentication and achieve control-flow hijacking without crashing the system.

## Questions for the full paper

- Which speculative gadget verifies the PAC, and how is the outcome observed?
- What had to be reverse-engineered on M1, and with which tools?
- Which defenses would close the attack without giving up PAC's performance?

## Connections

[GoFetch](chen-2024-gofetch.md) · [Interrupt side channels on Apple Silicon](zhang-2026-apple-interrupt-side-channels.md) · [Spectre](kocher-2019-spectre.md)
