---
id: "jattke-2022-blacksmith"
title: "Blacksmith: Scalable Rowhammering in the Frequency Domain"
authors: ["Patrick Jattke", "Victor van der Veen", "Pietro Frigo", "Stijn Gunter", "Kaveh Razavi"]
year: 2022
venue: "IEEE S&P 2022"
doi: "10.1109/SP46214.2022.9833772"
source: "https://ieeexplore.ieee.org/document/9833772/"
status: "catalogued"
topics: ["memory-systems", "dependable-computing", "physical-security"]
added: "2026-11-04"
source_checked: "2026-11-04"
read_version: null
---
# Blacksmith

## Source and seminar role

Seminar role: Citation-only supporting literature.

[Publication page](https://ieeexplore.ieee.org/document/9833772/) · [Publication DOI](https://doi.org/10.1109/SP46214.2022.9833772) · [Public PDF](https://comsec-files.ethz.ch/papers/blacksmith_sp22.pdf) · [Author project](https://comsec.ethz.ch/research/dram/blacksmith/) · [Author artifact](https://github.com/comsec-group/blacksmith)

Source limitations (UNVERIFIED): No matching arXiv record was verified.

Link check: The publication DOI and title match the publisher-deposited Crossref record. Publisher-page content is UNVERIFIED because automated access was restricted. The linked public PDF is accessible.

### Summary and evidence

Blacksmith represents the timing of non-uniform DRAM accesses in the frequency domain, as described in the abstract and project notes. Real DDR4 testing shows that mitigation effectiveness depends on the temporal structure of accesses, not just the number of aggressor rows.

### Place in the seminar

- Citation-only background: follow TRRespass with the role of non-uniform access patterns.
- Provide conceptual context for GPUThor without adding another deep-read requirement.

### Limits of the evidence

Results concern the tested memory sample and patterns. The method does not imply universal compromise of every DDR4 system or equivalent behavior in GDDR6.

Source check (2026-11-04): Author paper abstract, project page and publisher-deposited DOI record. Local reproduction is NOT_TESTED. Full reading remains unrecorded.

### Connections

[TRRespass](frigo-2020-trrespass.md) · [GPUThor](lin-2026-gputhor.md)

[Direction catalogue](index.md) · [Seminar overview](../seminar/README.md)
