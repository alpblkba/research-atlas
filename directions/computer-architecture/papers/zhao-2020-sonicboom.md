---
id: "zhao-2020-sonicboom"
title: "SonicBOOM: The 3rd Generation Berkeley Out-of-Order Machine"
authors: ["Jerry Zhao", "Ben Korpan", "Abraham Gonzalez", "Krste Asanović"]
year: 2020
venue: "CARRV 2020 workshop"
doi: null
source: "https://people.eecs.berkeley.edu/~krste/papers/SonicBOOM-CARRV2020.pdf"
status: "catalogued"
topics: ["computer-architecture", "microarchitectural-security"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# SonicBOOM

[Source](https://people.eecs.berkeley.edu/~krste/papers/SonicBOOM-CARRV2020.pdf) · [CARRV 2020 slides](https://carrv.github.io/2020/slides/CARRV2020_slides_15_Zhao.pdf) · [BOOM repository](https://github.com/riscv-boom/riscv-boom) · [Direction catalogue](index.md)

## Reading focus

SonicBOOM gives me synthesizable out-of-order RISC-V RTL. That matters for a speculation study where the timing of an actual pipeline stage enters the security argument.

- Attributes measured IPC gains to specific changes (a TAGE-based fetch unit, a load-store unit that issues multiple loads per cycle), which is a concrete account of where performance comes from in an OoO core.
- Same ISA as rv32i-mla with a very different microarchitecture, so it is the comparison point when deciding how far to grow the in-order design.

Reading tier: core.

## Source record

Source check by agent, 2026-11-06: abstract from the author PDF; venue taken from the CARRV 2020 slide archive.

The author PDF abstract was checked. The authors describe SonicBOOM as the third BOOM generation and as the highest-IPC open-source out-of-order design at publication time, attribute the gains to execution-path optimizations, a redesigned fetch unit with a TAGE predictor and a load-store unit that can issue multiple loads per cycle, and report about twice the SPEC CPU IPC of prior open-source OoO cores and 6.2 CoreMark/MHz. These are author-reported numbers from their own evaluation. The PDF does not print its venue; the CARRV 2020 attribution comes from the workshop slide archive.

## Questions for the full paper

- Which numbers come from RTL simulation, FireSim or silicon, and with which benchmark configuration?
- Where does speculative state live (ROB, load-store unit, branch snapshots), and what is squashed on a misprediction?
- What would it take to instrument the load-store unit to log transient loads?

## Connections

[The microarchitecture of superscalar processors](smith-1995-superscalar-microarchitecture.md) · [TAGE branch prediction](seznec-2006-tage.md) · [Chipyard](amid-2020-chipyard.md) · [FireSim](karandikar-2018-firesim.md) · [Unique program execution checking (UPEC)](../../microarchitectural-security/papers/fadiheh-2019-upec.md)
