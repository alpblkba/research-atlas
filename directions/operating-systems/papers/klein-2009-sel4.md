---
id: "klein-2009-sel4"
title: "seL4: Formal Verification of an OS Kernel"
authors: ["Gerwin Klein", "Kevin Elphinstone", "Gernot Heiser", "June Andronick", "David Cock", "Philip Derrin", "Dhammika Elkaduwe", "Kai Engelhardt", "Rafal Kolanski", "Michael Norrish", "Thomas Sewell", "Harvey Tuch", "Simon Winwood"]
year: 2009
venue: "SOSP 2009, pp. 207-220"
doi: "10.1145/1629575.1629596"
source: "https://doi.org/10.1145/1629575.1629596"
status: "catalogued"
topics: ["operating-systems"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# SeL4

[Publication DOI](https://doi.org/10.1145/1629575.1629596) · [Direction catalogue](index.md)

## Reading focus

For seL4 I want the exact boundary of the machine-checked proof. Which behavior follows from the kernel implementation, and which parts still depend on boot code, compiler and hardware assumptions?

- The proof's hardware assumptions are where the architecture directions meet microkernel work.
- Pairs with Verus to compare an interactive-proof project with an SMT-based one.

Reading tier: core.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: a machine-checked proof that the C implementation of a general-purpose microkernel matches its abstract specification.

## Questions for the full paper

- Which components are outside the proof (assembly, boot, caches, TLB management), and why?
- What did the proof cost in effort and proof size relative to the code size?
- How do later seL4 results (binary verification, timing channels) move the 2009 boundary?

## Connections

[Improving IPC by kernel design](liedtke-1993-improving-ipc.md) · [Verus](lattuada-2024-verus.md) · [ISA semantics in Sail](../../computer-architecture/papers/armstrong-2019-isa-semantics-sail.md)
