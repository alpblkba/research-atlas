---
id: "guthaus-2016-openram"
title: "OpenRAM: An Open-Source Memory Compiler"
authors: ["Matthew R. Guthaus", "James E. Stine", "Samira Ataei", "Brian Chen", "Bin Wu", "Mehedi Sarwar"]
year: 2016
venue: "ICCAD 2016, pp. 1-6"
doi: "10.1145/2966986.2980098"
source: "https://doi.org/10.1145/2966986.2980098"
status: "catalogued"
topics: ["computer-architecture", "memory-systems"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# OpenRAM

[Publication DOI](https://doi.org/10.1145/2966986.2980098) · [Direction catalogue](index.md)

## Reading focus

Laxity depends on where an SRAM bank sits. The PUF work depends on its state at power-up. OpenRAM is where I can look at how the array, its banks and its ports are built.

- One of the building blocks of open-source silicon flows on open PDKs.
- A memory compiler makes the cost of extra ports and banks explicit, which matters before proposing per-bank telemetry or partitioning in hardware.

Reading tier: optional; read when circuit-level SRAM questions come up.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: OpenRAM is an open-source compiler that generates, characterizes and verifies fabricable memory designs across technologies, meant to fill the gap left by limited PDK memory compilers and costly commercial tools.

## Questions for the full paper

- Which SRAM organizations are supported (port counts, banking), and which are left out?
- How is characterization done, and how close is it to commercial compilers?
- What has changed in later OpenRAM releases relative to the 2016 paper?

## Connections

[FPGA intrinsic PUFs](../../physical-security/papers/guajardo-2007-fpga-intrinsic-pufs.md) · [MemGuard](../../memory-systems/papers/yun-2013-memguard.md)
