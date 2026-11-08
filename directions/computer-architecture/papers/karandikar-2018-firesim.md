---
id: "karandikar-2018-firesim"
title: "FireSim: FPGA-Accelerated Cycle-Exact Scale-Out System Simulation in the Public Cloud"
authors: ["Sagar Karandikar", "Howard Mao", "Donggyu Kim", "David Biancolin", "Alon Amid", "Dayeol Lee", "Nathan Pemberton", "Emmanuel Amaro", "Colin Schmidt", "Aditya Chopra", "Qijing Huang", "Kyle Kovacs", "Borivoje Nikolić", "Randy Katz", "Jonathan Bachrach", "Krste Asanović"]
year: 2018
venue: "ISCA 2018, pp. 29-42"
doi: "10.1109/ISCA.2018.00014"
source: "https://doi.org/10.1109/ISCA.2018.00014"
status: "catalogued"
topics: ["computer-architecture"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# FireSim

[Publication DOI](https://doi.org/10.1109/ISCA.2018.00014) · [Direction catalogue](index.md)

## Reading focus

In FireSim the FPGA hosts the simulation. In rv32i-mla the design runs on the board itself. I want to keep those two timing measurements separate when comparing FPGA results.

- Cycle-exact simulation that boots Linux makes it possible to add a hardware feature and observe what the OS does with it, the measurement loop that hardware-assisted memory telemetry would need.
- Its decoupling of target time from host time is the methodological point to understand before trusting any FPGA-based performance number.

Reading tier: core for methodology.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: FireSim runs cycle-exact simulations of large clusters on FPGAs in the public cloud, with the stated aim of making large-scale hardware/software co-design affordable and easy to use.

## Questions for the full paper

- How does token-based decoupling keep the simulation cycle-exact when host FPGA timing differs from target timing?
- Which components are modeled abstractly (network, DRAM timing) and which are full RTL?
- What simulation rate is reported, and what does it imply for workload length?

## Connections

[Chipyard](amid-2020-chipyard.md) · [SonicBOOM](zhao-2020-sonicboom.md) · [Enzian](cock-2022-enzian.md)
