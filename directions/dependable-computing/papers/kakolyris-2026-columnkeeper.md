---
id: "kakolyris-2026-columnkeeper"
title: "ColumnKeeper: Efficient Solutions to the ColumnDisturb Vulnerability in DRAM-based Systems"
authors: ["Andreas Kosmas Kakolyris", "F. Nisa Bostanci", "Ataberk Olgun", "Ismail Emir Yuksel", "Harsh Songara", "Konstantinos Marios Sgouras", "Umut Baser", "Konstantinos Kanellopoulos", "A. Giray Yaglikci", "Onur Mutlu"]
year: 2026
venue: "ISCA 2026"
doi: "10.1109/ISCA66397.2026.00113"
source: "https://arxiv.org/abs/2606.22632v2"
status: "catalogued"
topics: ["memory-systems", "dependable-computing", "physical-security"]
added: "2026-11-04"
source_checked: "2026-11-04"
read_version: null
---
# ColumnKeeper

## Source and seminar role

Seminar role: Citation-only supporting literature.

[Publication page](https://ieeexplore.ieee.org/document/11617717/) · [Publication DOI](https://doi.org/10.1109/ISCA66397.2026.00113) · [arXiv v2](https://arxiv.org/abs/2606.22632v2) · [arXiv DOI](https://doi.org/10.48550/arXiv.2606.22632) · [Public PDF](https://arxiv.org/pdf/2606.22632v2) · [Author artifact](https://github.com/CMU-SAFARI/ColumnKeeper)

Link check: The publication DOI and title match the publisher-deposited Crossref record. Publisher-page content is UNVERIFIED because automated access was restricted. The linked public PDF is accessible.

### Summary and evidence

The v2 abstract gives two ways to schedule preventive refresh for ColumnDisturb, one deterministic and one probabilistic. Both use subarray/column organization to distribute preventive refreshes beyond the few adjacent rows assumed by conventional RowHammer defenses. Evaluation combines security analysis with modeled performance, energy and area.

### Place in the seminar

- Citation-only, use if needed: show an architectural response to the assumption challenged by ColumnDisturb.
- Keep this follow-up subordinate to the five core papers.

### Limits of the evidence

Simulated cost and guarantees depend on the ColumnDisturb threshold, subarray organization and chosen variant. Do not treat the design evaluation as measured deployment or as an interchangeable RowHammer threshold.

Source check (2026-11-04): arXiv v2 abstract, ISCA publication metadata and author artifact record. Full reading remains unrecorded.

### Connections

[ColumnDisturb](yuksel-2025-columndisturb.md)

[Direction catalogue](index.md) · [Seminar overview](../seminar/README.md)
