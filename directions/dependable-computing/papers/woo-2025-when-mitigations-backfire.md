---
id: "woo-2025-when-mitigations-backfire"
title: "When Mitigations Backfire: Timing Channel Attacks and Defense for PRAC-Based RowHammer Mitigations"
authors: ["Jeonghyun Woo", "Joyce Qu", "Gururaj Saileshwar", "Prashant J. Nair"]
year: 2025
venue: "ISCA 2025"
doi: "10.1145/3695053.3731007"
source: "https://arxiv.org/abs/2505.10111v3"
status: "catalogued"
topics: ["memory-systems", "dependable-computing", "physical-security"]
added: "2026-11-03"
source_checked: "2026-11-04"
read_version: null
---
# When Mitigations Backfire

[Source: arXiv v3](https://arxiv.org/abs/2505.10111v3) · [ISCA 2025 conference paper](https://gururaj-s.github.io/assets/pdf/ISCA25_Woo.pdf) · [Rowhammer comparison](../../memory-systems/rowhammer-mitigations.md)

## Evidence from the abstract

With PRAC, Alert Back-Off (ABO) and Refresh Management (RFM) can change observable request timing. The authors study what those changes reveal. They call the resulting attack family PRACLeak and propose TPRAC, which issues periodic Timing-Based RFMs instead of depending on observed activations. The abstract reports 3.4% slowdown at a Rowhammer threshold of 1024 for their evaluated setup. These are author-reported findings, not independent measurements by this vault.

## Reading lens

- Which resources are shared across attacker and victim, and what does the attacker actually observe? Distinguish a timing side channel from a Rowhammer bit flip.
- Trace the argument from row-activation counts to ABO/RFM commands and visible service delay. Locate the threat model and the point at which assumptions about mapping/co-location enter.
- Does activity-independent scheduling remove all timing variations or only the ones produced by the specified PRAC mechanism? What DRAM queue/controller changes and workload assumptions are involved?
- Record exact evaluation workload, baseline, threshold and overhead definition before comparing 3.4% with QPRAC's numbers.

## Relation and next action

[QPRAC](woo-2025-qprac.md) emphasizes mitigating Rowhammer efficiently; this paper tests what a PRAC mitigation reveals through shared timing. Do not treat either paper's word 'secure' as referring automatically to both properties. Comparison worksheet.

Reading state: Catalogued, abstract and source record checked. Full-paper notes and section/page anchors still pending.

## Catalogue update, 4 November 2026

Seminar role: Core seminar literature.

[Publication page](https://dl.acm.org/doi/10.1145/3695053.3731007) · [Publication DOI](https://doi.org/10.1145/3695053.3731007) · [arXiv v3](https://arxiv.org/abs/2505.10111v3) · [arXiv DOI](https://doi.org/10.48550/arXiv.2505.10111) · [Public PDF](https://gururaj-s.github.io/assets/pdf/ISCA25_Woo.pdf) · [Author artifact](https://github.com/STAR-Laboratory/PRAC_TC_ISCA25)

Link check: The publication DOI and title match the publisher-deposited Crossref record. Publisher-page content is UNVERIFIED because automated access was restricted. The linked public PDF is accessible.

### Summary and evidence

PRAC activation tracking can prevent disturbance while revealing activity through ABO/RFM-induced memory delays. The paper evaluates PRACLeak timing channels and activity-independent Timing-Safe PRAC (TPRAC). Its evidence is simulation-based; it is not an end-to-end demonstration on a deployed PRAC DDR5 system.

### Place in the seminar

- Core, deep reading: the central case of a protection mechanism introducing a different security exposure.
- Connect activation tracking and mitigation scheduling to timing confidentiality and performance.
- The published Ramulator2 artifact remains the first seminar demonstration candidate.

### Limits of the evidence

The reported 3.4% TPRAC overhead at N_RH = 1024 belongs to the evaluated workload and baseline. Do not generalize the channel closure claim to all memory timing channels or treat simulated PRACLeak results as physical bit-flip evidence.

Source check (2026-11-04): arXiv v3 abstract, author conference PDF evaluation/methodology and source record; existing reading questions retained. Full reading remains unrecorded.

### Connections

[QPRAC](woo-2025-qprac.md) · [LeakyHammer](bostanci-2025-leakyhammer.md)

[Direction catalogue](index.md) · [Seminar overview](../seminar/README.md) · [Seminar reading note](../seminar/papers/woo-2025-when-mitigations-backfire.md)
