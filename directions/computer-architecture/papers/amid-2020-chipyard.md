---
id: "amid-2020-chipyard"
title: "Chipyard: Integrated Design, Simulation, and Implementation Framework for Custom SoCs"
authors: ["Alon Amid", "David Biancolin", "Abraham Gonzalez", "Daniel Grubb", "Sagar Karandikar", "Harrison Liew", "Albert Magyar", "Howard Mao", "Albert J. Ou", "Nathan Pemberton", "Paul Rigge", "Colin Schmidt", "John Wright", "Jerry Zhao", "Yakun Sophia Shao", "Krste Asanović", "Borivoje Nikolić"]
year: 2020
venue: "IEEE Micro 40, pp. 10-21"
doi: "10.1109/MM.2020.2996616"
source: "https://doi.org/10.1109/MM.2020.2996616"
status: "catalogued"
topics: ["computer-architecture", "accelerators"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Chipyard

[Publication DOI](https://doi.org/10.1109/MM.2020.2996616) · [Direction catalogue](index.md)

## Reading focus

Chipyard is where Rocket, BOOM and Gemmini meet the rest of a RISC-V SoC. I want to see which integration decisions are already made before I change a core or accelerator.

- Its generator approach, one source producing RTL simulation, FPGA and VLSI targets, is the structured version of what rv32i-mla does by hand in a single Vivado block design.
- Defines the evaluation loop that FireSim then accelerates.

Reading tier: background; read for the flow and the simulation targets.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: Chipyard is an open-source framework that unifies design, simulation and physical implementation of custom SoCs using reusable generators, with FPGA and ASIC flows intended to keep validation continuous across stages.

## Questions for the full paper

- Which simulation targets are supported, and what does each cost per simulated cycle?
- How is a custom accelerator attached (RoCC versus memory-mapped TileLink), and what does the choice imply for the software interface?
- Where can plain Verilog modules be integrated without writing Chisel?

## Connections

[SonicBOOM](zhao-2020-sonicboom.md) · [FireSim](karandikar-2018-firesim.md) · [Gemmini](../../accelerators/papers/genc-2021-gemmini.md)
