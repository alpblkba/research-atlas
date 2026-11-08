---
id: "mueller-2023-automated-masking-fpga"
title: "Automated Masking of FPGA-Mapped Designs"
authors: ["Nicolai Müller", "Sergej Meschkov", "Dennis R. E. Gnad", "Mehdi B. Tahoori", "Amir Moradi"]
year: 2023
venue: "FPL 2023, 79–85"
doi: "10.1109/FPL60245.2023.00019"
source: "https://doi.org/10.1109/FPL60245.2023.00019"
status: "catalogued"
topics: ["physical-security", "compilers-and-runtimes"]
added: "2026-11-03"
source_checked: "2026-11-03"
read_version: null
---
# Automated masking of FPGA-mapped designs

[Source: KITopen](https://publikationen.bibliothek.kit.edu/1000165801) · [FPL 2023 DOI](https://doi.org/10.1109/FPL60245.2023.00019) · [Physical security direction](../index.md)

## Source-level result

AGEMA_FPGA adapts AGEMA's automatic masked-circuit generation to FPGA mapping. Their published abstract emphasizes LUT/register overhead and side-channel evaluation instead of assuming that an ASIC-oriented masking implementation maps efficiently to FPGAs. Area and power reductions are relative to the described AGEMA baseline; they should not be generalized without the design and benchmark details.

## Questions worth keeping

- Which transformations occur before versus after applying masking, and what properties must survive LUT mapping?
- What baseline and FPGA resources explain the reported area/power improvements?
- How does the side-channel evaluation test the security model, and what threat classes remain outside it?

This is a predecessor/context source for [Meschkov et al. 2025](meschkov-2025-secure-fpga-toolchain.md), not another required CDNC Rowhammer reading.

Reading state: Catalogued, abstract-level note only.
