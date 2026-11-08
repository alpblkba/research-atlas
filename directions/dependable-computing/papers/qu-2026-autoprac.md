---
id: "qu-2026-autoprac"
title: "AutoPRAC: Automating Attack Discovery for PRAC-Based Rowhammer Defenses using Model Checkers"
authors: ["Joyce Qu", "Gururaj Saileshwar"]
year: 2026
venue: "DRAMSec 2026 workshop"
doi: "10.48550/arXiv.2606.23905"
source: "https://arxiv.org/abs/2606.23905v1"
status: "catalogued"
topics: ["memory-systems", "dependable-computing", "physical-security"]
added: "2026-11-04"
source_checked: "2026-11-04"
read_version: null
---
# AutoPRAC

## Source and seminar role

Seminar role: Citation-only supporting literature.

[Publication page](https://dramsec.ethz.ch/) · [arXiv v1](https://arxiv.org/abs/2606.23905v1) · [arXiv DOI](https://doi.org/10.48550/arXiv.2606.23905) · [Public PDF](https://dramsec.ethz.ch/dramsec26-papers/AutoPRAC.dramsec26-final3.pdf)

Source limitations (UNVERIFIED): No separate proceedings DOI or public paper-specific repository was verified; the linked arXiv DOI identifies the preprint.

### Summary and evidence

AutoPRAC models a PRAC implementation as a bounded state machine, then searches for a reachable state that violates a stated safety property. The authors identify a counter-reset flaw in the modeled MOAT design that can leave up to 34 activations unaccounted for beyond the threshold.

### Place in the seminar

- Citation-only: illustrate automated scrutiny of counting/reset policies.
- Complement Chronus's simulation-fidelity example with formal-model counterexample discovery.

### Limits of the evidence

This is a workshop study and a bounded-model result, not a proof covering every implementation or a measured physical-memory exploit. MOAT is the analyzed mechanism here, not an extra paper added to the seminar set.

Source check (2026-11-04): DRAMSec program/paper and arXiv v1 abstract. Full reading remains unrecorded.

### Connections

[Chronus](canpolat-2025-chronus.md) · [QPRAC](woo-2025-qprac.md)

[Direction catalogue](index.md) · [Seminar overview](../seminar/README.md)
