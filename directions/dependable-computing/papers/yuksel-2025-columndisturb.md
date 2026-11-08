---
id: "yuksel-2025-columndisturb"
title: "ColumnDisturb: Understanding Column-based Read Disturbance in Real DRAM Chips and Implications for Future Systems"
authors: ["İsmail Emir Yüksel", "Ataberk Olgun", "F. Nisa Bostancı", "Haocong Luo", "A. Giray Yağlıkçı", "Onur Mutlu"]
year: 2025
venue: "MICRO 2025"
doi: "10.1145/3725843.3756022"
source: "https://arxiv.org/abs/2510.14750v2"
status: "catalogued"
topics: ["memory-systems", "dependable-computing", "physical-security"]
added: "2026-11-04"
source_checked: "2026-11-04"
read_version: null
---
# ColumnDisturb

## Source and seminar role

Seminar role: Citation-only supporting literature.

[Publication page](https://dl.acm.org/doi/10.1145/3725843.3756022) · [Publication DOI](https://doi.org/10.1145/3725843.3756022) · [arXiv v2](https://arxiv.org/abs/2510.14750v2) · [arXiv DOI](https://doi.org/10.48550/arXiv.2510.14750) · [Public PDF](https://arxiv.org/pdf/2510.14750v2) · [Institutional record, access UNVERIFIED](https://www.research-collection.ethz.ch/entities/publication/009d0832-b334-45f2-bbe2-08e905a93047)

Source limitations (UNVERIFIED): No separate paper-specific public repository was verified.

Link check: The publication DOI and title match the publisher-deposited Crossref record. Publisher-page content is UNVERIFIED because automated access was restricted. The linked public PDF is accessible.

### Summary and evidence

ColumnDisturb follows disturbance along bitlines across subarrays. The authors characterize the effect on 216 DDR4 chips and four HBM2 chips. A single aggressor can affect cells sharing columns across as many as three subarrays, unlike conventional nearby-row disturbance.

### Place in the seminar

- Citation-only: question the locality assumptions used to choose which victims need refresh.
- Keep the RowHammer survey bounded while acknowledging a distinct disturbance mechanism.

### Limits of the evidence

Column-based disturbance is not identical to RowHammer. Up to 3072 affected rows is a tested spatial extent, not a universal number of faults or proof that activation counters count incorrectly. The paper includes conditions beyond ordinary refresh windows; retain those conditions when citing results.

Source check (2026-11-04): arXiv v2 abstract and indexed institutional publication record. Direct access to the institutional page remains UNVERIFIED because it returned HTTP 500. Full reading remains unrecorded.

### Connections

[ColumnKeeper](kakolyris-2026-columnkeeper.md)

[Direction catalogue](index.md) · [Seminar overview](../seminar/README.md)
