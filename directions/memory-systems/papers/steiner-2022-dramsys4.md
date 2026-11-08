---
id: "steiner-2022-dramsys4"
title: "DRAMSys4.0: An Open-Source Simulation Framework for In-depth DRAM Analyses"
authors: ["Lukas Steiner", "Matthias Jung", "Felipe S. Prado", "Kirill Bykov", "Norbert Wehn"]
year: 2022
venue: "International Journal of Parallel Programming 50(2), pp. 217-242"
doi: "10.1007/s10766-022-00727-4"
source: "https://doi.org/10.1007/s10766-022-00727-4"
status: "catalogued"
topics: ["memory-systems"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# DRAMSys4.0

[Publication DOI](https://doi.org/10.1007/s10766-022-00727-4) · [Direction catalogue](index.md)

## Reading focus

DRAMSys gives me an independent SystemC TLM model to compare with Ramulator 2. A difference between their results is a reason to inspect the configuration and timing assumptions.

- Supports DDR5 and LPDDR5, which matters for PRAC-era studies.
- Comes from the RPTU Kaiserslautern microelectronic systems group, one of the European groups working on DRAM controllers and memory architecture.

Reading tier: background.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: a fast, open-source DRAM simulator based on transaction-level modeling that supports recent JEDEC standards such as DDR5 and LPDDR5, compared with other simulators.

## Questions for the full paper

- What does TLM-based simulation give up in accuracy for its speed, compared with cycle-level simulators?
- Which power and thermal models are included?
- Has any PRAC or RFM result been reproduced in both DRAMSys and Ramulator2?

## Connections

[Ramulator 2.0](luo-2024-ramulator2.md) · [Memory access scheduling](rixner-2000-memory-access-scheduling.md)
