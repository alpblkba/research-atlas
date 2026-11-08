---
id: "luo-2024-ramulator2"
title: "Ramulator 2.0: A Modern, Modular, and Extensible DRAM Simulator"
authors: ["Haocong Luo", "Yahya Can Tuğrul", "F. Nisa Bostancı", "Ataberk Olgun", "A. Giray Yağlıkçı", "Onur Mutlu"]
year: 2024
venue: "IEEE Computer Architecture Letters 23(1), pp. 112-116"
doi: "10.1109/LCA.2023.3333759"
source: "https://doi.org/10.1109/LCA.2023.3333759"
status: "catalogued"
topics: ["memory-systems", "dependable-computing"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Ramulator 2.0

[Publication DOI](https://doi.org/10.1109/LCA.2023.3333759) · [Direction catalogue](index.md)

## Reading focus

UNVERIFIED against the paper: the technical description below is provisional. The source check covered the bibliographic listing, not the full text or abstract.

The WMB artifact uses Ramulator 2. Before interpreting a latency plot, I need to know which controller and DRAM behaviors come from the simulator and which ones the paper adds.

- Describes the modular structure that PRAC and RFM experiments modify.
- Methodology reference for memory controller experiments that do not need RTL.

Reading tier: core for the seminar artifact.

## Source record

Source check by agent, 2026-11-06: metadata from Crossref; the record has no abstract, so the summary below is the agent's and is UNVERIFIED against the paper.

The record carries no abstract. Agent summary: the letter describes Ramulator 2.0's modular design, which separates DRAM specifications, controller behavior and mitigation mechanisms so that new standards and RowHammer mitigations can be added as plugins.

## Questions for the full paper

- Which DRAM standards and mitigations ship in the release used by the WMB artifact?
- How is timing validated, and against which reference?
- What does the simulator not model, and how does that bound what a seminar demonstration can claim?

## Connections

[When Mitigations Backfire](../../dependable-computing/papers/woo-2025-when-mitigations-backfire.md) · [DRAMSys4.0](steiner-2022-dramsys4.md) · [Flipping bits in memory without accessing them](kim-2014-flipping-bits.md)
