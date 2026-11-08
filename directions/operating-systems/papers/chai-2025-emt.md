---
id: "chai-2025-emt"
title: "EMT: An OS Framework for New Memory Translation Architectures"
authors: ["Siyuan Chai", "Jiyuan Zhang", "Jongyul Kim", "Alan Wang", "Fan Chung", "Jovan Stojkovic", "Weiwei Jia", "Dimitrios Skarlatos", "Josep Torrellas", "Tianyin Xu"]
year: 2025
venue: "OSDI 2025, pp. 711-729"
doi: null
source: "https://www.usenix.org/conference/osdi25/presentation/chai-siyuan"
status: "catalogued"
topics: ["operating-systems", "memory-systems", "computer-architecture"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# EMT

[Source](https://www.usenix.org/conference/osdi25/presentation/chai-siyuan) · [Direction catalogue](index.md)

## Reading focus

EMT gives Linux a hardware-neutral interface for address translation. That makes it possible to ask how a proposed MMU behaves under a real OS without rebuilding Linux memory management for every design.

- Sits on the hardware/OS boundary for virtual memory and connects Direct Segments-style architecture work to kernel implementation.
- From Tianyin Xu's group at UIUC with Torrellas and Skarlatos, linking the SREGym context to architecture/OS co-design.

Reading tier: core.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the USENIX presentation page.

USENIX abstract: EMT is a Linux-based layer that offers a hardware-neutral interface for diverse translation designs, including tree-based and hash-based ones, and the authors use it to add OS support for two experimental schemes, ECPT and FPT.

## Questions for the full paper

- Which abstraction does EMT expose, and what does it cost relative to stock Linux?
- Which OS-level problems did implementing ECPT and FPT reveal that simulation had hidden?
- Could EMT host a segment-based scheme such as Direct Segments?

## Connections

[Efficient virtual memory for big memory servers (direct segments)](basu-2013-direct-segments.md) · [TPP](maruf-2023-tpp.md) · [Demystifying CXL memory](../../memory-systems/papers/sun-2023-demystifying-cxl.md) · [SREGym](../../systems-reliability/papers/clark-2026-sregym.md)
