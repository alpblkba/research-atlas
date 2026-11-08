---
id: "kim-2025-prac-real-hardware"
title: "Per-Row Activation Counting on Real Hardware: Demystifying Performance Overheads"
authors: ["Jumin Kim", "Seungmin Baek", "Minbok Wi", "Hwayong Nam", "Michael Jaemin Kim", "Sukhan Lee", "Kyomin Sohn", "Jung Ho Ahn"]
year: 2025
venue: "IEEE Computer Architecture Letters 2025"
doi: "10.1109/LCA.2025.3587293"
source: "https://arxiv.org/abs/2507.05556v2"
status: "catalogued"
topics: ["memory-systems", "dependable-computing", "physical-security"]
added: "2026-11-04"
source_checked: "2026-11-04"
read_version: null
---
# PRAC on real hardware

## Source and seminar role

Seminar role: Citation-only supporting literature.

[Publication page](https://ieeexplore.ieee.org/document/11074718/) · [Publication DOI](https://doi.org/10.1109/LCA.2025.3587293) · [arXiv v2](https://arxiv.org/abs/2507.05556v2) · [arXiv DOI](https://doi.org/10.48550/arXiv.2507.05556) · [Public PDF](https://arxiv.org/pdf/2507.05556v2) · [Author publication note](https://geniajh.github.io/post/202507-cal-prac.html)

Source limitations (UNVERIFIED): No public paper-specific code repository was verified.

Link check: The publication DOI and title match the publisher-deposited Crossref record. Publisher-page content is UNVERIFIED because automated access was restricted. The linked public PDF is accessible.

### Summary and evidence

On the Intel systems in this study, the authors change DRAM timing parameters to reflect PRAC and then run SPEC CPU2017. Section IV reports 1.06% mean and 3.28% maximum overhead with prefetching enabled in the evaluated configuration, and examines row-buffer/page-policy effects.

### Place in the seminar

- Citation-only: anchor the timing-cost discussion in measurements on real machines.
- Explain the timing-model error corrected by Chronus and why different workload/controller assumptions produce different overheads.

### Limits of the evidence

This is a timing-only experiment: it does not deploy PRAC per-row tracking, ALERT or RFM behavior. It is not a full-mitigation cost measurement. arXiv v2 (1 November 2025) explicitly acknowledges the Chronus correction; its earlier comparison numbers must not replace corrected Chronus results.

Source check (2026-11-04): arXiv v2 abstract, introduction and Section IV, plus CAL DOI record. Full reading remains unrecorded.

### Connections

[Chronus](canpolat-2025-chronus.md) · [CnC-PRAC](lin-2025-cnc-prac.md)

[Direction catalogue](index.md) · [Seminar overview](../seminar/README.md)
