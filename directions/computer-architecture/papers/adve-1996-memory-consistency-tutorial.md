---
id: "adve-1996-memory-consistency-tutorial"
title: "Shared Memory Consistency Models: A Tutorial"
authors: ["Sarita V. Adve", "Kourosh Gharachorloo"]
year: 1996
venue: "IEEE Computer 29, pp. 66-76"
doi: "10.1109/2.546611"
source: "https://doi.org/10.1109/2.546611"
status: "catalogued"
topics: ["computer-architecture", "operating-systems"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Shared memory consistency models

[Publication DOI](https://doi.org/10.1109/2.546611) · [Direction catalogue](index.md)

## Reading focus

UNVERIFIED against the paper: the technical description below is provisional. The source check covered the bibliographic listing, not the full text or abstract.

Coherence tells me about copies of a location. To reason about the order in which different locations become visible, I also need the memory consistency model that the core, compiler and kernel share.

- Explains why sequential consistency is expensive and what relaxed models allow, which is the background for Arm's weak ordering on Apple Silicon compared with x86 TSO.
- Kernel synchronization, lock-free code and DMA buffer handoff all rely on fences whose meaning comes from this model.

Reading tier: core.

## Source record

Source check by agent, 2026-11-06: metadata from Crossref; the record has no abstract, so the summary below is the agent's and is UNVERIFIED against the paper.

The record carries no abstract. Agent summary: the tutorial defines sequential consistency, shows how common hardware optimizations violate it, and presents relaxed models through a programmer-centric view.

## Questions for the full paper

- Which hardware optimizations (write buffers, overlapped writes, non-blocking reads) break sequential consistency, and in which examples?
- How does the programmer-centric view relate to the C11 and C++11 memory models?
- Which of the described relaxations does RISC-V RVWMO permit?

## Connections

[The Multikernel](../../operating-systems/papers/baumann-2009-multikernel.md) · [ISA semantics in Sail](armstrong-2019-isa-semantics-sail.md)
