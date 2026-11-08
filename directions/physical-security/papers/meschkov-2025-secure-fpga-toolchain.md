---
id: "meschkov-2025-secure-fpga-toolchain"
title: "Design and Implementation of a Physically Secure Open-Source FPGA and Toolchain"
authors: ["Sergej Meschkov", "Daniel Lammers", "Mehdi B. Tahoori", "Amir Moradi"]
year: 2025
venue: "IACR TCHES 2025(3), 542–582"
doi: "10.46586/tches.v2025.i3.542-582"
source: "https://publikationen.bibliothek.kit.edu/1000184046"
status: "catalogued"
topics: ["physical-security", "compilers-and-runtimes", "dependable-computing"]
added: "2026-11-03"
source_checked: "2026-11-03"
read_version: null
---
# Physically secure open-source FPGA and toolchain

[Source: KITopen](https://publikationen.bibliothek.kit.edu/1000184046) · [TCHES 2025 DOI](https://doi.org/10.46586/tches.v2025.i3.542-582) · [Physical security direction](../index.md)

## Evidence from the abstract

Meschkov, Lammers, Tahoori and Moradi treat the fabric and mapping toolchain as one physical-security design. The case study combines masking/hiding for side-channel resistance with fault-injection detection; the described primitives use modified LMDPL and WDDL ideas. The authors report an experimental TVLA evaluation and area comparison. These are abstract-level author claims, not proof that every mapped HDL circuit has no practical leakage.

## Questions for Sergej's research context

- What is the boundary of the stated security guarantees: secure primitive, composition, mapped design, physical board, or all of them under specified assumptions?
- How does the mapping flow preserve masking independence and avoid glitches/transition leakage after technology mapping?
- Which properties are mathematically derived and which are supported by board-level TVLA? What cannot a TVLA non-detection establish?
- How do configurability, area cost and protection assumptions differ from conventional FPGA tools?

Read this to understand CDNC's electrical/implementation perspective, not as a Rowhammer paper. Related: [automated masking (FPL 2023)](mueller-2023-automated-masking-fpga.md), [PWNN (TCHES 2026)](xu-2026-pwnn.md).

Reading state: Catalogued and abstract checked; Introduction and implementation sections pending.
