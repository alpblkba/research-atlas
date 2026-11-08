---
id: "coalson-2024-prisonbreak"
title: "PrisonBreak: Jailbreaking Large Language Models with at Most Twenty-Five Targeted Bit-flips"
authors: ["Zachary Coalson", "Jeonghyun Woo", "Chris S. Lin", "Joyce Qu", "Yu Sun", "Shiyang Chen", "Lishan Yang", "Gururaj Saileshwar", "Prashant Nair", "Bo Fang", "Sanghyun Hong"]
year: 2024
venue: "arXiv preprint (v3 revised 2025)"
doi: "10.48550/arXiv.2412.07192"
source: "https://arxiv.org/abs/2412.07192v3"
status: "catalogued"
topics: ["memory-systems", "dependable-computing", "physical-security"]
added: "2026-11-04"
source_checked: "2026-11-04"
read_version: null
---
# PrisonBreak

## Source and seminar role

Seminar role: Citation-only supporting literature.

[arXiv v3](https://arxiv.org/abs/2412.07192v3) · [arXiv DOI](https://doi.org/10.48550/arXiv.2412.07192) · [Public PDF](https://arxiv.org/pdf/2412.07192v3) · [Author publication list](https://www.zachcoalson.com/)

Source limitations (UNVERIFIED): No peer-reviewed publication DOI or public paper-specific repository was verified; the linked arXiv DOI identifies the preprint.

### Summary and evidence

PrisonBreak asks whether changing a small set of model parameters can change which requests an LLM refuses. The current v3 reports 5-25 bit-flip model evaluations and a GDDR6 RowHammer demonstration, separating hardware-agnostic model effects from hardware-aware exploitation.

### Place in the seminar

- Citation-only: distinguish alignment integrity from classification accuracy and code integrity.
- Contrast the model-parameter target with PRowhammer's host-side GPU-library target.

### Limits of the evidence

Section 3 starts with a white-box model and a co-located user-level GPU process. Section 6.4 also studies black-box transfer between related models, so "white-box only" is too strong. v1 dates to December 2024; use v3 (2 October 2025) for current title/authors and GDDR6 results. Do not attribute v3 results retroactively to v1.

Source check (2026-11-04): arXiv v3 abstract, threat model and Section 6.4; author publication record. Full reading remains unrecorded.

### Connections

[PRowhammer](shukla-2026-prowhammer.md) · [GPUHammer](lin-2025-gpuhammer.md)

[Direction catalogue](index.md) · [Seminar overview](../seminar/README.md)
