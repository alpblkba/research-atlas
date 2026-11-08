---
id: "lin-2026-gpubreach"
title: "GPUBreach: Privilege Escalation Attacks on GPUs using Rowhammer"
authors: ["Chris S. Lin", "Yuqin Yan", "Guozhen Ding", "Joyce Qu", "Joseph Zhu", "David Lie", "Gururaj Saileshwar"]
year: 2026
venue: "IEEE S&P 2026"
doi: "10.1109/SP63933.2026.00177"
source: "https://arxiv.org/abs/2605.03812v2"
status: "catalogued"
topics: ["memory-systems", "dependable-computing", "physical-security"]
added: "2026-11-04"
source_checked: "2026-11-04"
read_version: null
---
# GPUBreach

## Source and seminar role

Seminar role: Optional research pool.

[Publication page](https://ieeexplore.ieee.org/document/11573424/) · [Publication DOI](https://doi.org/10.1109/SP63933.2026.00177) · [arXiv v2](https://arxiv.org/abs/2605.03812v2) · [arXiv DOI](https://doi.org/10.48550/arXiv.2605.03812) · [Public PDF](https://gururaj-s.github.io/assets/pdf/SP26_GPUBreach.pdf) · [Author artifact](https://github.com/sith-lab/gpubreach)

Link check: The publication DOI and title match the publisher-deposited Crossref record. Publisher-page content is UNVERIFIED because automated access was restricted. The linked public PDF is accessible.

### Summary and evidence

In the NVIDIA configuration studied here, corruption of GPU page tables compromises isolation on the GPU and has consequences for the host. Evidence includes real-hardware and end-to-end system experiments.

### Place in the seminar

- Optional pool: use only if the survey needs a contrast between model corruption and memory-isolation failure.
- Provide a GPU-to-CPU counterpart to PRowhammer's CPU-to-GPU dependency.

### Limits of the evidence

It is not a sixth core paper or an added artifact task. The GPU/driver configuration and ECC assumptions bound the result; GPUThor's ECC-enabled claims are a separate study.

Source check (2026-11-04): arXiv/publication abstract, author PDF and artifact record. Full reading remains unrecorded.

### Connections

[GPUHammer](lin-2025-gpuhammer.md) · [PRowhammer](shukla-2026-prowhammer.md) · [GPUThor](lin-2026-gputhor.md)

[Direction catalogue](index.md) · [Seminar overview](../seminar/README.md)
