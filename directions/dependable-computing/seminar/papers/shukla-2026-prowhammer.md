---
id: "shukla-2026-prowhammer"
title: "PRowhammer: Propagating Bit-Flips from CPU to GPU"
authors: ["Mrityunjay Shukla", "Shubham Roy", "Sayandeep Saha", "Biswabandan Panda"]
year: 2026
venue: "ISCA 2026"
doi: "10.1109/ISCA66397.2026.00116"
source: "https://ieeexplore.ieee.org/document/11617762/"
status: "catalogued"
topics: ["memory-systems", "dependable-computing", "physical-security"]
added: "2026-11-04"
source_checked: "2026-11-04"
read_version: null
---
# PRowhammer

Seminar role: Core seminar literature, deep reading.

The [direction paper note](../../papers/shukla-2026-prowhammer.md) is the maintained source for metadata, verified links, summary, evidence and caveats. I keep the seminar questions here and use the direction note for citations.

## Summary and reading focus

PRowhammer studies how a co-resident unprivileged CPU process can corrupt GPU-library code in host DRAM and affect GPU execution. Shared host-memory library pages and valid-but-altered GPU instructions connect CPU-memory integrity to classification and language-model outcomes. The paper reports DDR3/DDR4 physical-fault experiments and application-impact evaluations.

## Place in the seminar

- Core, deep reading: expose the dependency of GPU execution on host DRAM and shared libraries.
- Contrast code-integrity failures with the model-weight corruption studied in GPUHammer and PrisonBreak.

## Evidence and caveats

Section V-A requires a co-resident unprivileged CPU process; black-box refers to knowledge of the model, not a remote-API-only attacker. Section VI explicitly retains the relevance of CPU-side RowHammer defenses, including PRAC/TPRAC. A controlled corruption demonstration is different from reproducing the physical RowHammer stage.

[Source links and verification status](../../papers/shukla-2026-prowhammer.md#source-and-seminar-role) · [Full evidence note](../../papers/shukla-2026-prowhammer.md#summary-and-evidence)

Reading state: Catalogued as core; this entry does not mark a completed user full read.

[Seminar paper index](index.md) · [Seminar overview](../README.md) · [Direction catalogue](../../papers/index.md)
