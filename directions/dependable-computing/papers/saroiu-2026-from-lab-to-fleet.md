---
id: "saroiu-2026-from-lab-to-fleet"
title: "From Lab to Fleet: Building and Deploying a Practical Rowhammer Defense in Cloud SoCs"
authors: ["Stefan Saroiu", "Sujay Yadalam", "Alec Wolman", "Will Remaklus", "Daniel Berger", "Isaac H. Luna", "Ishwar Agarwal", "Jacob R. Lorch"]
year: 2026
venue: "ISCA 2026 industry track"
doi: "10.1109/ISCA66397.2026.00062"
source: "https://ieeexplore.ieee.org/document/11617830/"
status: "catalogued"
topics: ["memory-systems", "dependable-computing", "physical-security"]
added: "2026-11-04"
source_checked: "2026-11-04"
read_version: null
---
# Sigries / From Lab to Fleet

## Source and seminar role

Seminar role: Citation-only supporting literature.

[Publication page](https://ieeexplore.ieee.org/document/11617830/) · [Publication DOI](https://doi.org/10.1109/ISCA66397.2026.00062) · [Public PDF](https://stefan.t8k2.com/publications/isca/2026/sigries-with-errata.pdf) · [Microsoft publication](https://www.microsoft.com/en-us/research/publication/from-lab-to-fleet-building-and-deploying-a-practical-rowhammer-defense-in-cloud-socs/) · [Author errata](https://www.microsoft.com/en-us/research/wp-content/uploads/2026/06/sigries-errata.pdf)

Source limitations (UNVERIFIED): No matching arXiv record or public paper-specific repository was verified. The Microsoft PDF button leads to an errata-only page; use the full author PDF for the paper.

Link check: The publication DOI and title match the publisher-deposited Crossref record. Publisher-page content is UNVERIFIED because automated access was restricted. The linked public PDF is accessible.

### Summary and evidence

Sigries runs in the memory controller of Azure Cobalt 200. It combines limited Misra-Gries tracking with a row-sampling fallback. The deployment account and trace-driven evaluation emphasize hardware cost, liveness and predictable overhead.

### Place in the seminar

- Citation-only: represent production constraints in a seminar otherwise dominated by research designs.
- Pair with FiRM to discuss mode-transition assumptions and subsequent correction.

### Limits of the evidence

Use the full author PDF with the August 2026 errata on page 16. The errata retracts the claim that heavy-to-light transitions are always safe and discusses hardware/configuration fixes. This is not evidence that the entire deployed fleet was experimentally compromised; the public performance evaluation is trace-driven.

Source check (2026-11-04): Microsoft abstract, full author PDF abstract and page 16 errata (also visually checked). Full reading remains unrecorded.

### Connections

[FiRM / From Fleet to Lab](taneja-2026-from-fleet-to-lab.md)

[Direction catalogue](index.md) · [Seminar overview](../seminar/README.md)
