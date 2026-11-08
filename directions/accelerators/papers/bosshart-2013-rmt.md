---
id: "bosshart-2013-rmt"
title: "Forwarding Metamorphosis: Fast Programmable Match-Action Processing in Hardware for SDN"
authors: ["Pat Bosshart", "Glen Gibb", "Hun-Seok Kim", "George Varghese", "Nick McKeown", "Martin Izzard", "Fernando Mujica", "Mark Horowitz"]
year: 2013
venue: "SIGCOMM 2013, pp. 99-110"
doi: "10.1145/2486001.2486011"
source: "https://doi.org/10.1145/2486001.2486011"
status: "catalogued"
topics: ["accelerators", "operating-systems"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Forwarding metamorphosis (RMT)

[Publication DOI](https://doi.org/10.1145/2486001.2486011) · [Direction catalogue](index.md)

## Reading focus

RMT gives me a hardware model for P4. A packet goes through a sequence of configurable match and action stages. The interesting constraint is what each stage can finish before the next packet arrives.

- Connects SDN and data-plane networking to accelerator architecture by asking what programmability costs in silicon.

Reading tier: optional; read for network data-plane silicon.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: a reconfigurable match-tables model and pipelined switch architecture let programmers change how packet headers are processed, argued to be feasible at almost no extra cost or power.

## Questions for the full paper

- How are match tables mapped onto SRAM and TCAM across pipeline stages?
- What area and power overhead is claimed, and against which fixed-function baseline?
- Which limits of the model motivated later work such as P4 and its compilers?

## Connections

[The eXpress Data Path (XDP)](../../operating-systems/papers/hoiland-jorgensen-2018-xdp.md) · [MLIR](../../compilers-and-runtimes/papers/lattner-2021-mlir.md)
