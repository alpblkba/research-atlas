---
id: "abgrall-2026-jenga"
title: "JENGA: Exploiting Counter-Based RowHammer Countermeasures to Break Real-Time Predictability"
authors: ["Valentin Abgrall", "Marcello Traiola", "Ruben Salvador", "Maria Méndez Real", "Alessandro Palumbo", "Angeliki Kritikakou"]
year: 2026
venue: "IEEE RTSS 2026 (accepted; forthcoming on 2026-11-04)"
doi: "10.48550/arXiv.2609.01077"
source: "https://arxiv.org/abs/2609.01077v1"
status: "catalogued"
topics: ["memory-systems", "dependable-computing", "physical-security"]
added: "2026-11-04"
source_checked: "2026-11-04"
read_version: null
---
# JENGA

## Source and seminar role

Seminar role: Optional research pool.

[arXiv v1](https://arxiv.org/abs/2609.01077v1) · [arXiv DOI](https://doi.org/10.48550/arXiv.2609.01077) · [Public PDF](https://arxiv.org/pdf/2609.01077v1)

Source limitations (UNVERIFIED): No proceedings DOI or public paper-specific repository was verified; the linked arXiv DOI identifies the preprint.

### Summary and evidence

The JENGA v1 abstract asks what a counter-based RowHammer defense does to the execution-time bound a real-time task relies on. The arXiv v1 abstract describes JENGA as an analysis of counter-based RowHammer mitigation and real-time execution guarantees. gem5/Ramulator 2.0 experiments with TACLeBench show mitigation-induced timing variation; the paper derives a bound that accounts for these delays in WCET analysis.

### Place in the seminar

- Optional pool: distinguish worst-case predictability from the average-performance metrics in PRAC studies.
- A short comparison is sufficient if real-time guarantees become relevant to the discussion.

### Limits of the evidence

Simulation and analytical bounds are not measurements of a deployed real-time DDR5 system. This is the 2026 RowHammer/WCET paper, not the unrelated older Jenga work on stacked-DRAM fault tolerance. No new real-time-system scope or experiment is implied.

Source check (2026-11-04): arXiv v1 abstract and publication-status record. Full reading remains unrecorded.

### Connections

[When Mitigations Backfire](woo-2025-when-mitigations-backfire.md) · [Chronus](canpolat-2025-chronus.md)

[Direction catalogue](index.md) · [Seminar overview](../seminar/README.md)
