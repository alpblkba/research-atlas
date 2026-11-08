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

## Source and seminar role

Seminar role: Core seminar literature.

[Publication page](https://ieeexplore.ieee.org/document/10946773/) · [Publication DOI](https://doi.org/10.1109/HPCA61900.2025.00071) · [arXiv v2](https://arxiv.org/abs/2502.12650v2) · [arXiv DOI](https://doi.org/10.48550/arXiv.2502.12650) · [Public PDF](https://arxiv.org/pdf/2502.12650v2) · [Corrected full text](https://arxiv.org/html/2502.12650v2) · [Author artifact](https://github.com/CMU-SAFARI/Chronus)

Link check: The publication DOI and title match the publisher-deposited Crossref record. Publisher-page content is UNVERIFIED because automated access was restricted. The linked public PDF is accessible.

### Summary and evidence

Chronus separates two costs in PRAC: updating the counters and reacting quickly enough to a wave of activations. The authors propose Concurrent Counter Update and a dynamic back-off policy. It separates counters from data accesses and varies preventive refresh work. Evidence combines security analysis, Ramulator 2.0 simulation, and energy/area modeling.

### Place in the seminar

- Core, deep reading with emphasis on analysis: connect RowHammer thresholds to PRAC security and scaling cost.
- Understand CCU and Chronus Back-Off conceptually to distinguish design-dependent overhead from an unavoidable counting cost.
- Use the corrected results as a concrete example of evaluation fidelity.

### Limits of the evidence

Use arXiv v2 (7 September 2025), not the original abstract. Section 6.1/Figure 4 and Appendix E/Table 4 correct PRAC timing reductions for tRAS, tRTP and tWR. For four-core PRAC-4 at N_RH = 1024, average performance overhead changes from 9.7% to 5.8% (corrected maximum 8.9%). Corrected averages at N_RH = 64 and 20 are 8.1% and 78.5%. These are simulated overheads over the paper's baseline, not the timing-only real-machine measurement.

Source check (2026-11-04): arXiv v2 abstract, Sections 6.1 and 7, and Appendix E/Table 4. Full reading remains unrecorded.

### Connections

[PRAC on real hardware](kim-2025-prac-real-hardware.md) · [CnC-PRAC](lin-2025-cnc-prac.md) · [QPRAC](woo-2025-qprac.md)

[Direction catalogue](index.md) · [Seminar overview](../seminar/README.md) · [Seminar reading note](../seminar/papers/canpolat-2025-chronus.md)
