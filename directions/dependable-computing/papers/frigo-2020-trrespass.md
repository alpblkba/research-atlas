---
id: "frigo-2020-trrespass"
title: "TRRespass: Exploiting the Many Sides of Target Row Refresh"
authors: ["Pietro Frigo", "Emanuele Vannacci", "Hasan Hassan", "Victor van der Veen", "Onur Mutlu", "Cristiano Giuffrida", "Herbert Bos", "Kaveh Razavi"]
year: 2020
venue: "IEEE S&P 2020"
doi: "10.1109/SP40000.2020.00090"
source: "https://arxiv.org/abs/2004.01807v1"
status: "catalogued"
topics: ["memory-systems", "dependable-computing", "physical-security"]
added: "2026-11-04"
source_checked: "2026-11-04"
read_version: null
---
# TRRespass

## Source and seminar role

Seminar role: Citation-only supporting literature.

[Publication page](https://ieeexplore.ieee.org/document/9152631/) · [Publication DOI](https://doi.org/10.1109/SP40000.2020.00090) · [arXiv v1](https://arxiv.org/abs/2004.01807v1) · [arXiv DOI](https://doi.org/10.48550/arXiv.2004.01807) · [Public PDF](https://download.vusec.net/papers/trrespass_sp20.pdf) · [Author project](https://www.vusec.net/projects/trrespass/) · [Author artifact](https://github.com/vusec/trrespass)

Link check: The publication DOI and title match the publisher-deposited Crossref record. Publisher-page content is UNVERIFIED because automated access was restricted. The linked public PDF is accessible.

### Summary and evidence

In the paper abstract and project description, repeated accesses across multiple aggressors exceed what the opaque TRR implementation can track. The study combines FPGA-assisted characterization with real-system tests and reports vulnerable DDR4 modules and LPDDR4(X) devices.

### Place in the seminar

- Citation-only background: explain why TRR did not settle the RowHammer problem.
- Introduce the difference between a marketing-level protection claim and a tested implementation guarantee.

### Limits of the evidence

The reported 13 vulnerable modules out of 42 tested DDR4 modules describes that sample, not all DDR4 or all TRR designs. Keep TRR distinct from newer per-row counting frameworks.

Source check (2026-11-04): Publication metadata, author project and arXiv abstract. Local reproduction is NOT_TESTED. Full reading remains unrecorded.

### Connections

[Blacksmith](jattke-2022-blacksmith.md) · [QPRAC](woo-2025-qprac.md)

[Direction catalogue](index.md) · [Seminar overview](../seminar/README.md)
