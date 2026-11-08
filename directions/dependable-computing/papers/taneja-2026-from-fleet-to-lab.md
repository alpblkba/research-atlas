---
id: "taneja-2026-from-fleet-to-lab"
title: "From Fleet to Lab: Revisiting the Security and Complexity of Industrial Rowhammer Mitigation"
authors: ["Hritvik Taneja", "Moinuddin Qureshi"]
year: 2026
venue: "arXiv preprint"
doi: "10.48550/arXiv.2608.26072"
source: "https://arxiv.org/abs/2608.26072v1"
status: "catalogued"
topics: ["memory-systems", "dependable-computing", "physical-security"]
added: "2026-11-04"
source_checked: "2026-11-04"
read_version: null
---
# FiRM / From Fleet to Lab

## Source and seminar role

Seminar role: Citation-only supporting literature.

[arXiv v1](https://arxiv.org/abs/2608.26072v1) · [arXiv DOI](https://doi.org/10.48550/arXiv.2608.26072) · [Public PDF](https://arxiv.org/pdf/2608.26072v1) · [Author publication list](https://hritwik567.github.io/)

Source limitations (UNVERIFIED): No peer-reviewed publication DOI or public paper-specific repository was verified; the linked arXiv DOI identifies the preprint.

### Summary and evidence

The authors examine what happens when Sigries switches modes and propose two variants of Filtered Rowhammer Mitigation (FiRM), one probabilistic and one deterministic. It co-designs tracking and sampling budgets and uses SRAM filters to reduce tracking complexity. Evidence is analytical security modeling plus performance simulation.

### Place in the seminar

- Citation-only: follow the deployed-design description with a critique of transition guarantees.
- Distinguish security of each operating mode from security of their composition.

### Limits of the evidence

Section II-E states that deployed Sigries parameters are undisclosed and its analysis estimates/infers them. The approximately one-second MTTF is an analytical result for stated assumptions, not an observed Azure fleet failure or demonstrated production compromise. Read together with Sigries's own errata.

Source check (2026-11-04): arXiv v1 abstract, Sections II-E and III, and author publication list. Full reading remains unrecorded.

### Connections

[Sigries / From Lab to Fleet](saroiu-2026-from-lab-to-fleet.md)

[Direction catalogue](index.md) · [Seminar overview](../seminar/README.md)
