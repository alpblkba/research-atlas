---
id: "cock-2022-enzian"
title: "Enzian: An Open, General, CPU/FPGA Platform for Systems Software Research"
authors: ["David Cock", "Abishek Ramdas", "Daniel Schwyn", "Michael J. Giardino", "Adam Turowski", "Zhenhao He", "Nora Hossle", "Dario Korolija", "Melissa Licciardello", "Kristina Martsenko", "Reto Achermann", "Gustavo Alonso", "Timothy Roscoe"]
year: 2022
venue: "ASPLOS 2022, pp. 434-451"
doi: "10.1145/3503222.3507742"
source: "https://doi.org/10.1145/3503222.3507742"
status: "catalogued"
topics: ["computer-architecture", "operating-systems"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Enzian

[Publication DOI](https://doi.org/10.1145/3503222.3507742) · [Direction catalogue](index.md)

## Reading focus

UNVERIFIED against the paper: the technical description below is provisional. The source check covered the bibliographic listing, not the full text or abstract.

Enzian connects an FPGA to the server CPU through its coherence protocol. That makes it a plausible platform for a memory-side prototype whose state the OS can observe.

- Built so that systems software researchers can change the hardware beneath them, which is the hardware/OS boundary in physical form.
- A useful contrast with FireSim: real CPU silicon plus an FPGA, against a fully simulated target.

Reading tier: optional.

## Source record

Source check by agent, 2026-11-06: metadata from OpenAlex; the record has no abstract, so the summary below is the agent's and is UNVERIFIED against the paper.

The record carries no abstract. Agent summary: the paper describes the Enzian research computer, its coherent CPU/FPGA interconnect, and the system software and use cases built on it.

## Questions for the full paper

- What does the FPGA see of the coherence protocol, and at what latency?
- Which experiments in the paper would be impossible with a PCIe-attached FPGA?
- How available is the platform to groups outside ETH?

## Connections

[FireSim](karandikar-2018-firesim.md) · [Dune](../../operating-systems/papers/belay-2012-dune.md) · [Demystifying CXL memory](../../memory-systems/papers/sun-2023-demystifying-cxl.md)
