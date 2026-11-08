---
id: "seshadri-2017-ambit"
title: "Ambit: In-Memory Accelerator for Bulk Bitwise Operations Using Commodity DRAM Technology"
authors: ["Vivek Seshadri", "Donghyuk Lee", "Thomas Mullins", "Hasan Hassan", "Amirali Boroumand", "Jeremie Kim", "Michael A. Kozuch", "Onur Mutlu", "Phillip B. Gibbons", "Todd C. Mowry"]
year: 2017
venue: "MICRO 2017, pp. 273-287"
doi: "10.1145/3123939.3124544"
source: "https://doi.org/10.1145/3123939.3124544"
status: "catalogued"
topics: ["memory-systems", "accelerators"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Ambit

[Publication DOI](https://doi.org/10.1145/3123939.3124544) · [Direction catalogue](index.md)

## Reading focus

UNVERIFIED against the paper: the technical description below is provisional. The source check covered the bibliographic listing, not the full text or abstract.

Ambit uses charge sharing during multi-row activation to compute in DRAM. That's a useful physical connection to the disturbance literature, although the intended operation and failure condition differ.

- The FHE seminar work studied processing near memory (FHEmem); Ambit is the in-DRAM end of that design space and a baseline for what minimal DRAM changes can do.
- Treats data movement as the measured quantity, the same lens as the FHE data-movement note.

Reading tier: background.

## Source record

Source check by agent, 2026-11-06: metadata from Crossref; the record has no abstract, so the summary below is the agent's and is UNVERIFIED against the paper.

The record carries no abstract. Agent summary: Ambit performs bulk bitwise AND, OR and NOT inside DRAM using simultaneous multi-row activation and dual-contact cells, with small changes to the DRAM array and the controller.

## Questions for the full paper

- Which DRAM changes are required, and what do they cost in area?
- How does triple-row activation interact with reliability and disturbance?
- What does the evaluation assume about data layout and OS support?

## Connections

[FHEmem](../../accelerators/papers/zhou-2023-fhemem.md) · [Flipping bits in memory without accessing them](kim-2014-flipping-bits.md) · [FHE data movement](../../accelerators/fhe-data-movement.md)
