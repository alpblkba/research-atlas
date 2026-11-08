---
id: "shukla-2026-prowhammer"
title: "PRowhammer: Propagating Bit-Flips from CPU to GPU"
authors: ["Mrityunjay Shukla", "Shubham Roy", "Sayandeep Saha", "Biswabandan Panda"]
year: 2026
venue: "ISCA 2026"
doi: "10.1109/ISCA66397.2026.00116"
source: "https://ieeexplore.ieee.org/document/11617762/"
status: "catalogued"
topics: ["memory-systems", "dependable-computing", "physical-security"]
added: "2026-11-04"
source_checked: "2026-11-04"
read_version: null
---
# PRowhammer

## Source and seminar role

Seminar role: Core seminar literature.

[Publication page](https://ieeexplore.ieee.org/document/11617762/) · [Publication DOI](https://doi.org/10.1109/ISCA66397.2026.00116) · [Public PDF](https://www.cse.iitb.ac.in/~biswa/ISCA2026.pdf) · [Archived artifact DOI](https://doi.org/10.5281/zenodo.19326669) · [Artifact record](https://zenodo.org/records/19326669)

Source limitations (UNVERIFIED): No matching arXiv record was verified.

Link check: The publication DOI and title match the publisher-deposited Crossref record. Publisher-page content is UNVERIFIED because automated access was restricted. The linked public PDF is accessible.

### Summary and evidence

PRowhammer starts on the host. An unprivileged co-resident CPU process can corrupt GPU-library code in host DRAM, changing what later executes on the GPU. Shared host-memory library pages and valid-but-altered GPU instructions connect CPU-memory integrity to classification and language-model outcomes. The paper reports DDR3/DDR4 physical-fault experiments and application-impact evaluations.

### Place in the seminar

- Core, deep reading: expose the dependency of GPU execution on host DRAM and shared libraries.
- Contrast code-integrity failures with the model-weight corruption studied in GPUHammer and PrisonBreak.

### Limits of the evidence

Section V-A requires a co-resident unprivileged CPU process; black-box refers to knowledge of the model, not a remote-API-only attacker. Section VI explicitly retains the relevance of CPU-side RowHammer defenses, including PRAC/TPRAC. A controlled corruption demonstration is different from reproducing the physical RowHammer stage.

Source check (2026-11-04): Author PDF abstract, Sections V-A and VI, and artifact appendix; DOI metadata and Zenodo record checked. Archive files were not downloaded or executed. Full reading remains unrecorded.

### Connections

[GPUHammer](lin-2025-gpuhammer.md) · [PrisonBreak](coalson-2024-prisonbreak.md) · [When Mitigations Backfire](woo-2025-when-mitigations-backfire.md)

[Direction catalogue](index.md) · [Seminar overview](../seminar/README.md) · [Seminar reading note](../seminar/papers/shukla-2026-prowhammer.md)
