---
id: "armstrong-2019-isa-semantics-sail"
title: "ISA Semantics for ARMv8-A, RISC-V, and CHERI-MIPS"
authors: ["Alasdair Armstrong", "Thomas Bauereiss", "Brian Campbell", "Alastair Reid", "Kathryn E. Gray", "Robert M. Norton", "Prashanth Mundkur", "Mark Wassell", "Jon French", "Christopher Pulte", "Shaked Flur", "Ian Stark", "Neel Krishnaswami", "Peter Sewell"]
year: 2019
venue: "Proceedings of the ACM on Programming Languages 3 (POPL 2019), pp. 1-31"
doi: "10.1145/3290384"
source: "https://doi.org/10.1145/3290384"
status: "catalogued"
topics: ["computer-architecture", "microarchitectural-security"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# ISA semantics in Sail

[Publication DOI](https://doi.org/10.1145/3290384) · [Direction catalogue](index.md)

## Reading focus

For rv32i-mla, an executable ISA model gives me something precise to compare against after each instruction. Sail makes the architectural behavior explicit enough to do that comparison.

- Sail models back the RISC-V specification work, so this is where formal ISA verification meets everyday RTL testing.
- The CHERI model connects to the capability-hardware papers in the security directions.

Reading tier: core for the verification thread.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from Crossref.

Crossref abstract: the paper presents formal, executable sequential ISA models written in Sail for several architectures, complete enough to boot real operating systems.

## Questions for the full paper

- What is in scope (sequential semantics) and what is excluded (concurrency, timing, microarchitecture)?
- How is the model validated against hardware or reference simulators?
- Which tools generate test oracles or theorem-prover definitions from Sail?

## Connections

[Shared memory consistency models](adve-1996-memory-consistency-tutorial.md) · [Verus](../../operating-systems/papers/lattuada-2024-verus.md) · [Unique program execution checking (UPEC)](../../microarchitectural-security/papers/fadiheh-2019-upec.md) · [CHERIoT](../../microarchitectural-security/papers/amar-2023-cheriot.md)
