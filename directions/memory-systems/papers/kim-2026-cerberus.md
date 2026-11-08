---
id: "kim-2026-cerberus"
title: "Cerberus: Cross-Layer ECC Co-Design for Robust and Efficient Memory Protection"
authors: ["Junhwan Kim", "Seunghyun Kim", "Yesin Ryu", "Saeid Gorgin", "Jungrae Kim"]
year: 2026
venue: "ISCA 2026"
doi: null
source: "https://arxiv.org/abs/2605.02220v2"
status: "catalogued"
topics: ["memory-systems", "dependable-computing"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Cerberus

[Source](https://arxiv.org/abs/2605.02220v2) · [ISCA 2026 program](https://www.iscaconf.org/isca2026/program/) · [Direction catalogue](index.md)

## Reading focus

Cerberus looks at error correction across the die, the link and the system. Each layer sees a different part of the failure, so I want to follow one error through all three.

- Supplies the ECC side that the seminar touches only briefly, where GPUThor treats ECC as a finite correction capability.
- Listed in the ISCA 2026 best paper candidate session; an SKKU news release reports that it won the best paper award (secondary source, not the ISCA site).

Reading tier: optional, recent.

## Source record

Source check by agent, 2026-11-06: abstract from arXiv v2; venue from the ISCA 2026 program.

arXiv v2 abstract: Cerberus unifies on-die, link and system ECC through an encode-once, decode-many design in which one controller-side encoding serves all three layers; the authors report better resilience to clustered and peripheral faults with lower redundancy, targeting custom HBM. The ISCA 2026 program lists it in Session 1A. No DOI recorded yet.

## Questions for the full paper

- Which fault models are assumed, and do they come from field data or from models?
- What must change in DRAM devices and controllers, and is it compatible with JEDEC standards?
- How would cross-layer ECC change RowHammer threat models that rely on ECC miscorrection?

## Connections

[GPUThor](../../dependable-computing/papers/lin-2026-gputhor.md) · [Flipping bits in memory without accessing them](kim-2014-flipping-bits.md) · [Cores that don't count](../../systems-reliability/papers/hochschild-2021-cores-that-dont-count.md)
