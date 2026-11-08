---
id: "sapui-2024-memristor-cim-sidechannel"
title: "Side-Channel Attack with Fault Analysis on Memristor-based Computation-in-Memory"
authors: ["Brojogopal Sapui", "Sergej Meschkov", "Mehdi B. Tahoori"]
year: 2024
venue: "30th IEEE International Symposium on On-Line Testing and Robust System Design (IOLTS), 1–7"
doi: "10.1109/IOLTS60994.2024.10616088"
source: "https://doi.org/10.1109/IOLTS60994.2024.10616088"
status: "prior-work-imported"
topics: ["hardware-security", "memory-systems", "side-channels", "computation-in-memory"]
added: "2026-11-03"
source_checked: "2026-11-03"
read_version: null
---

# Side-Channel Attack with Fault Analysis on Memristor-based Computation-in-Memory

[Published conference paper](https://doi.org/10.1109/IOLTS60994.2024.10616088) · Uploaded source: `Side-Channel_Attack_with_Fault_Analysis_on_Memristor-based_Computation-in-Memory.pdf`

## Mechanism and evidence

Sapui, Meschkov and Tahoori examine the timing of scouting-logic operations in non-stateful memristor computation-in-memory circuits. The paper argues that variations in circuit response and fault sensitivity can disclose information even in a computation model designed to minimize data movement. Its case study uses a scouting-logic XOR circuit and evaluates a proposed configurable-delay hiding countermeasure. The results are based on a circuit-level and netlist-based simulation environment, including device-variation models, rather than a demonstrated attack against fabricated CiM hardware. The authors report correlation-analysis results and a first-order Test Vector Leakage Assessment (TVLA) on simulated protected and unprotected designs, including an evaluation at the scale of one million traces. An absence of detected first-order leakage in the modeled protected case is not a proof of security against every side channel, fault condition, technology variation or physical implementation.

## Details to check

- Distinguish stateful and non-stateful memristive logic and explain how scouting logic reads an output using peripheral current sensing (Section II).
- Identify the trust and measurement assumptions behind the paper's fault-sensitivity side channel; distinguish a simulated observable from one available on a packaged physical device (Sections II–III).
- Examine the authors' statistical evaluation criteria and note what the correlation results establish for the XOR case study versus what remains untested for larger cryptographic or ML workloads (Sections III and V).
- Understand the intended defensive role of the configurable-delay circuit and audit its area, power and timing trade-offs against the unprotected case (Sections IV–V).
- Record which cell models, variability assumptions and simulation tools underpin the evaluation; avoid treating nominal simulation results as independently characterized fabricated-device measurements (Section V).
- Separate the reported TVLA result, the chosen leakage model and higher-order or different physical observables before drawing security conclusions (Section V).

## Comparison

[MemFHE](https://doi.org/10.1145/3569955) is an RRAM-based FHE processing-in-memory accelerator, while [FHEmem](https://doi.org/10.48550/arXiv.2311.16293) proposes an HBM/DRAM near-mat CKKS accelerator. This paper studies a different memristive scouting-logic circuit and a specific modeled side channel. Shared use of the terms ReRAM, PIM or CiM does not show that the same leakage exists in those FHE accelerators; the device organization, supported operations and experimental assumptions must be checked separately.

Reading state: Uploaded IOLTS PDF inspected for the target circuit, modeled evaluation boundary, countermeasure and results; no physical-device replication or broader cryptographic-system vulnerability is claimed.
