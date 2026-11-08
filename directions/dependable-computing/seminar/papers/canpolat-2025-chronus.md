---
id: "canpolat-2025-chronus"
title: "Chronus: Understanding and Securing the Cutting-Edge Industry Solutions to DRAM Read Disturbance"
authors: ["Oğuzhan Canpolat", "A. Giray Yağlıkçı", "Geraldo F. Oliveira", "Ataberk Olgun", "Nisa Bostancı", "İsmail Emir Yüksel", "Haocong Luo", "Oğuz Ergin", "Onur Mutlu"]
year: 2025
venue: "HPCA 2025"
doi: "10.1109/HPCA61900.2025.00071"
source: "https://arxiv.org/abs/2502.12650v2"
status: "catalogued"
topics: ["memory-systems", "dependable-computing", "physical-security"]
added: "2026-11-04"
source_checked: "2026-11-04"
read_version: null
---
# Chronus

Seminar role: Core seminar literature, deep reading.

The [direction paper note](../../papers/canpolat-2025-chronus.md) is the maintained source for metadata, verified links, summary, evidence and caveats. I keep the seminar questions here and use the direction note for citations.

## Summary and reading focus

Chronus analyzes PRAC counter-update latency and wave-attack constraints, then proposes Concurrent Counter Update and dynamic back-off mitigation. It separates counters from data accesses and varies preventive refresh work. Evidence combines security analysis, Ramulator 2.0 simulation, and energy/area modeling.

## Place in the seminar

- Core, deep reading with emphasis on analysis: connect RowHammer thresholds to PRAC security and scaling cost.
- Understand CCU and Chronus Back-Off conceptually to distinguish design-dependent overhead from an unavoidable counting cost.
- Use the corrected results as a concrete example of evaluation fidelity.

## Evidence and caveats

Use arXiv v2 (7 September 2025), not the original abstract. Section 6.1/Figure 4 and Appendix E/Table 4 correct PRAC timing reductions for tRAS, tRTP and tWR. For four-core PRAC-4 at N_RH = 1024, average performance overhead changes from 9.7% to 5.8% (corrected maximum 8.9%). Corrected averages at N_RH = 64 and 20 are 8.1% and 78.5%. These are simulated overheads over the paper's baseline, not the timing-only real-machine measurement.

[Source links and verification status](../../papers/canpolat-2025-chronus.md#source-and-seminar-role) · [Full evidence note](../../papers/canpolat-2025-chronus.md#summary-and-evidence)

Reading state: Catalogued as core; this entry does not mark a completed user full read.

[Seminar paper index](index.md) · [Seminar overview](../README.md) · [Direction catalogue](../../papers/index.md)
