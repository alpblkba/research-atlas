---
id: "rixner-2000-memory-access-scheduling"
title: "Memory Access Scheduling"
authors: ["Scott Rixner", "William J. Dally", "Ujval J. Kapasi", "Peter Mattson", "John D. Owens"]
year: 2000
venue: "ISCA 2000"
doi: "10.1145/339647.339668"
source: "https://doi.org/10.1145/339647.339668"
status: "catalogued"
topics: ["memory-systems"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Memory access scheduling

[Publication DOI](https://doi.org/10.1145/339647.339668) · [Direction catalogue](index.md)

## Reading focus

UNVERIFIED against the paper: the technical description below is provisional. The source check covered the bibliographic listing, not the full text or abstract.

A controller can serve a later request first because its row is already open. That choice matters when I interpret queueing delays in an FR-FCFS model or a Ramulator-based PRAC study.

- Use the scheduling model as background when checking the controller assumptions in PRAC, RFM and QoS papers.
- Shows why a row-hit-first policy creates unfairness between threads, the problem that MISE and later QoS schedulers address.

Reading tier: core for memory systems.

## Source record

Source check by agent, 2026-11-06: metadata from Crossref; the record has no abstract, so the summary below is the agent's and is UNVERIFIED against the paper.

The record carries no abstract. Agent summary: the paper argues that reordering memory operations to exploit bank parallelism and row-buffer locality raises sustained bandwidth, and compares several scheduling policies on media-processing workloads.

## Questions for the full paper

- Which policies are compared, and with what workloads and DRAM model?
- Which fairness or starvation issues does the paper acknowledge?
- How do DDR5 constraints (bank groups, refresh management) change the conclusions?

## Connections

[MISE](subramanian-2013-mise.md) · [Ramulator 2.0](luo-2024-ramulator2.md) · [When Mitigations Backfire](../../dependable-computing/papers/woo-2025-when-mitigations-backfire.md)
