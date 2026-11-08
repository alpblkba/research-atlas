---
id: "lopes-2021-alive2"
title: "Alive2: Bounded Translation Validation for LLVM"
authors: ["Nuno P. Lopes", "Juneyoung Lee", "Chung-Kil Hur", "Zhengyang Liu", "John Regehr"]
year: 2021
venue: "PLDI 2021, pp. 65-79"
doi: "10.1145/3453483.3454030"
source: "https://doi.org/10.1145/3453483.3454030"
status: "catalogued"
topics: ["compilers-and-runtimes"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Alive2

[Publication DOI](https://doi.org/10.1145/3453483.3454030) · [Direction catalogue](index.md)

## Reading focus

Alive2 asks an SMT solver whether an LLVM transformation preserves the behavior it is supposed to preserve. Its bounds matter when interpreting both a counterexample and a successful check.

- The compilers direction asks whether properties survive transformations; Alive2 asks it for functional correctness, while the secure FPGA toolchain papers ask it for physical security.

Reading tier: background.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: Alive2 automatically checks LLVM IR transformations with an SMT solver within resource bounds; it found 47 new bugs (28 since fixed) and led to fixes in LLVM's semantics.

## Questions for the full paper

- What does bounded mean here (loop unrolling, memory size), and what can escape?
- How are undefined behavior and poison values modeled?
- Could the same approach validate an HDL synthesis step?

## Connections

[LLVM](lattner-2004-llvm.md) · [Verus](../../operating-systems/papers/lattuada-2024-verus.md) · [Physically secure open-source FPGA and toolchain](../../physical-security/papers/meschkov-2025-secure-fpga-toolchain.md)
