---
id: "lin-2025-cnc-prac"
title: "CnC-PRAC: Coalesce, not Cache, Per Row Activation Counts for an Efficient in-DRAM Rowhammer Mitigation"
authors: ["Chris S. Lin", "Jeonghyun Woo", "Prashant J. Nair", "Gururaj Saileshwar"]
year: 2025
venue: "DRAMSec 2025 workshop"
doi: "10.48550/arXiv.2506.11970"
source: "https://arxiv.org/abs/2506.11970v1"
status: "catalogued"
topics: ["memory-systems", "dependable-computing", "physical-security"]
added: "2026-11-04"
source_checked: "2026-11-04"
read_version: null
---
# CnC-PRAC

## Source and seminar role

Seminar role: Citation-only supporting literature.

[Publication page](https://dramsec.ethz.ch/2025.html) · [arXiv v1](https://arxiv.org/abs/2506.11970v1) · [arXiv DOI](https://doi.org/10.48550/arXiv.2506.11970) · [Public PDF](https://dramsec.ethz.ch/dramsec25-papers/cncprac-dramsec25.pdf)

Source limitations (UNVERIFIED): No separate proceedings DOI or public paper-specific repository was verified; the linked arXiv DOI identifies the preprint.

### Summary and evidence

CnC-PRAC groups updates before writing them to separate DRAM counter rows. Its buffer can reorder several pending updates to the same row. This builds on decoupled counter/data access to reduce counter-row activations and associated energy. Reported benefits come from simulation and modeling.

### Place in the seminar

- Citation-only: show that PRAC overhead depends on counter-storage and update design choices.
- Complement Chronus and the timing-only hardware study without promising a common simulator comparison.

### Limits of the evidence

The workshop evaluation predates Chronus's September 2025 errata. Do not assume the reported baseline is corrected or compare percentages directly without checking timing models, workload and energy accounting.

Source check (2026-11-04): DRAMSec paper and arXiv v1 abstract/source record. Full reading remains unrecorded.

### Connections

[Chronus](canpolat-2025-chronus.md) · [PRAC on real hardware](kim-2025-prac-real-hardware.md)

[Direction catalogue](index.md) · [Seminar overview](../seminar/README.md)
