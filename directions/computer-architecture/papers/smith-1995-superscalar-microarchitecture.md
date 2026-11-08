---
id: "smith-1995-superscalar-microarchitecture"
title: "The Microarchitecture of Superscalar Processors"
authors: ["James E. Smith", "Gurindar S. Sohi"]
year: 1995
venue: "Proceedings of the IEEE 83, pp. 1609-1624"
doi: "10.1109/5.476078"
source: "https://doi.org/10.1109/5.476078"
status: "catalogued"
topics: ["computer-architecture"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# The microarchitecture of superscalar processors

[Publication DOI](https://doi.org/10.1109/5.476078) · [Direction catalogue](index.md)

## Reading focus

UNVERIFIED against the paper: the technical description below is provisional. The source check covered the bibliographic listing, not the full text or abstract.

Before reading SonicBOOM I need to follow one instruction through rename, issue, the reorder buffer and commit. Otherwise it is easy to mistake a speculative result for an architectural one.

- The rv32i-mla core is a three-stage in-order design; this survey lays out which structures appear, and which problem each one solves, when a design moves from in-order issue to dynamic scheduling.
- Meltdown and Spectre are consequences of the speculation and in-order retirement described here, so the security directions depend on this background.

Reading tier: background; read the sections on instruction flow and on memory operations first.

## Source record

Source check by agent, 2026-11-06: metadata from OpenAlex; the record has no abstract, so the summary below is the agent's and is UNVERIFIED against the paper.

The record carries no abstract. Agent summary: a tutorial survey of superscalar organization covering instruction fetch and branch handling, register renaming, dynamic scheduling, the handling of loads and stores, and the mechanisms that keep exceptions precise.

## Questions for the full paper

- Which structures exist to keep exceptions precise, and which exist only for throughput?
- How does the paper treat load/store ordering hazards, and where does that reasoning reappear in a modern load-store unit?
- Which 1995 assumptions (issue width, clock targets, predictor accuracy) no longer hold, and does that change any argument?

## Connections

[TAGE branch prediction](seznec-2006-tage.md) · [SonicBOOM](zhao-2020-sonicboom.md) · [Meltdown](../../microarchitectural-security/papers/lipp-2018-meltdown.md)
