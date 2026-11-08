# CDNC dependable computing seminar, WS 2026/27

## Current seminar status, 4 November 2026

RowHammer Across Modern Memory Architectures: Attacks, Defenses, and AI Security

I have five papers in the core reading list. The final research question remains open until the core reading is complete.

KIT CDNC Dependable Computing Seminar, WS 2026/27, 3 ECTS. The deliverables are a survey paper, a 15-minute presentation, a selection rationale for each paper and an artifact presentation.

### Selected literature

The [core index](papers/index.md) contains WMB, QPRAC, Chronus, GPUHammer and PRowhammer. Reading order remains WMB, QPRAC, Chronus, GPUHammer, PRowhammer; QPRAC is the focused/short read. The [direction catalogue](../papers/index.md) also contains all 12 citation-only papers and the two optional pool entries.

### Scope and evidence

The focus remains RowHammer across CPU DRAM, GPU memory and AI integrity. ColumnDisturb is used to examine architectural assumptions, not to expand the survey to all DRAM disturbance mechanisms. Keep simulation, real-machine timing measurements, physical faults and application-level consequences distinct.

- WMB PRACLeak evidence is simulation-based.
- [Chronus](../papers/canpolat-2025-chronus.md) uses corrected arXiv v2, including Appendix E.
- [The real-hardware PRAC study](../papers/kim-2025-prac-real-hardware.md) measures timing changes, not deployed tracking/ALERT/RFM.
- [PRowhammer](../papers/shukla-2026-prowhammer.md) assumes a co-resident unprivileged CPU process; CPU-side defenses remain relevant.
- Compare each paper's metrics and assumptions; do not collapse them to a universal overhead number or claim a citation disconnect between communities.

### Existing artifact priority

WMB/Ramulator2 remains first; PRowhammer remains an optional later demonstration. The literature catalogue adds no experiment or common-simulator integration commitment. GPU access/compatibility for PRowhammer is still unconfirmed. Controlled corruption and physical RowHammer reproduction must be distinguished. No artifact was installed or run by this update.

## Earlier proposal

The following text records the earlier two-paper proposal and is preserved as historical context; the five-paper selection above is current.

Proposed subject: Security and performance trade-offs of architectural Rowhammer mitigations, anchored on When Mitigations Backfire and QPRAC.

## Seminar-specific reading subset

- [When Mitigations Backfire (ISCA 2025)](papers/woo-2025-when-mitigations-backfire.md): PRACLeak, timing channel, TPRAC.
- [QPRAC (HPCA 2025)](papers/woo-2025-qprac.md): prioritization and PRAC mitigation.

`papers/` contains deliberate copies of these two [dependable-computing paper notes](../papers/index.md), so the seminar subset is available on its own. The notes are catalogued, not represented as fully reviewed, and edits to copies will not automatically sync. Other Meschkov papers are contextual reading, not part of this requested seminar-only subset.

## Work products

- [Slides](slides/README.md) for seminar presentation files.
- [Assets](assets/README.md) for seminar diagrams and other supplementary material.
- Rowhammer literature comparison exercise stays in the general exercises directory until a graded deliverable is defined.

No simulator artifact or benchmark is included here. Any future implementation belongs in a separate repository; this directory holds reading and seminar writing only.

[Dependable computing direction](../index.md) · [Research Atlas](../../../README.md)
