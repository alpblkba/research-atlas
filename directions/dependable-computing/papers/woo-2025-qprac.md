---
id: "woo-2025-qprac"
title: "QPRAC: Towards Secure and Practical PRAC-based Rowhammer Mitigation using Priority Queues"
authors: ["Jeonghyun Woo", "Chris S. Lin", "Prashant J. Nair", "Aamer Jaleel", "Gururaj Saileshwar"]
year: 2025
venue: "HPCA 2025"
doi: "10.1109/HPCA61900.2025.00080"
source: "https://arxiv.org/abs/2501.18861v5"
status: "catalogued"
topics: ["memory-systems", "dependable-computing", "physical-security"]
added: "2026-11-03"
source_checked: "2026-11-04"
read_version: null
---
# QPRAC

[Source: arXiv v5](https://arxiv.org/abs/2501.18861v5) · [HPCA 2025 DOI](https://doi.org/10.1109/HPCA61900.2025.00080) · [Rowhammer comparison](../../memory-systems/rowhammer-mitigations.md)

## Evidence from the abstract

PRAC counts activations per row and uses Alert Back-Off (ABO) to request mitigation. QPRAC proposes a priority-based service queue to choose pending mitigations without requiring an oracle for the most activated rows. The design combines priority-based service with opportunistic RFM and proactive refresh-time mitigation. The authors report protection at very low Rowhammer thresholds (as low as 71) with 0.8% benign-workload slowdown, reduced to 0% under the described proactive policy. Those numbers are conditional author claims, not results measured here.

## Reading lens

- What information does the PSQ hold, and how does priority order affect the worst-case unmitigated activation count?
- Why are prior designs described as insecure or impractical? Record the exact oracular or on-chip state assumptions.
- Separate activations, pending mitigation actions, ABO/RFM events and host-visible slowdown; identify the baseline for each metric.
- Does the paper claim protection against physical Rowhammer disturbance, timing channels, or both? Do not import the latter property without evidence.

## Relation and next action

Read next to [When Mitigations Backfire](woo-2025-when-mitigations-backfire.md): both involve PRAC, but the paper's primary security question is different. The artifact [repository](https://github.com/sith-lab/qprac) is only a citation; no installation or execution is planned.

Reading state: Catalogued, abstract and bibliographic record checked. No full-paper critique yet.

## Catalogue update, 4 November 2026

Seminar role: Core seminar literature.

[Publication page](https://ieeexplore.ieee.org/document/10946754/) · [Publication DOI](https://doi.org/10.1109/HPCA61900.2025.00080) · [arXiv v5](https://arxiv.org/abs/2501.18861v5) · [arXiv DOI](https://doi.org/10.48550/arXiv.2501.18861) · [Public PDF](https://arxiv.org/pdf/2501.18861v5) · [Author artifact](https://github.com/sith-lab/qprac)

Link check: The publication DOI and title match the publisher-deposited Crossref record. Publisher-page content is UNVERIFIED because automated access was restricted. The linked public PDF is accessible.

### Summary and evidence

QPRAC uses a priority-based service queue to select rows for mitigation, coupled with reactive ABO and opportunistic/proactive refresh scheduling. Its security reasoning and simulated performance characterize a particular PRAC design; disturbance protection does not by itself establish timing confidentiality.

### Place in the seminar

- Core, focused/short reading: establish PRAC, ABO, RFM and mitigation-queue concepts needed for WMB.
- Explain how scheduling choices affect protection guarantees and benign-workload costs.

### Limits of the evidence

The abstract reports a threshold as low as 71 and 0.8% slowdown, reduced to 0% with the stated proactive policy. Keep configuration, baseline and workload attached to these claims; they are not a universal cost for PRAC.

Source check (2026-11-04): arXiv v5 abstract and publication/artifact records; existing detailed reading questions retained. Full reading remains unrecorded.

### Connections

[When Mitigations Backfire](woo-2025-when-mitigations-backfire.md) · [Chronus](canpolat-2025-chronus.md)

[Direction catalogue](index.md) · [Seminar overview](../seminar/README.md) · [Seminar reading note](../seminar/papers/woo-2025-qprac.md)
