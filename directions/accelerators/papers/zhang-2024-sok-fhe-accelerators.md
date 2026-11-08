---
id: "zhang-2024-sok-fhe-accelerators"
title: "SoK: Fully Homomorphic Encryption Accelerators"
authors: ["Junxue Zhang", "Xiaodian Cheng", "Liu Yang", "Jinbin Hu", "Ximeng Liu", "Kai Chen"]
year: 2024
venue: "ACM Computing Surveys 56(12), Article 316"
doi: "10.1145/3676955"
source: "https://arxiv.org/abs/2212.01713"
status: "prior-work-imported"
topics: ["accelerators", "memory-systems"]
added: "2026-11-03"
source_checked: "2026-11-03"
read_version: null
---
# SoK: Fully Homomorphic Encryption Accelerators

[Source: arXiv (first submitted 2022)](https://arxiv.org/abs/2212.01713) · [Published article](https://doi.org/10.1145/3676955) · [FHE comparison](../fhe-data-movement.md)

## Evidence from the source

The SoK compares existing FHE accelerator designs. It examines 14 named accelerator efforts across general-purpose processors, GPUs, FPGAs and ASICs, organizing their evolution around polynomial computation, ciphertext maintenance, hardware specialization and software/hardware co-design. The paper distinguishes expensive polynomial operations from key switching and bootstrapping, then combines a qualitative architectural survey with testbed measurements of representative open-source accelerators. For closed-source designs, some evaluation comparisons use numbers reported by the original publications rather than measurements reproduced on one common platform. The paper also discusses programmability, design trade-offs and scaling as directions for subsequent work.

## Details to check

- Reconstruct the paper's taxonomy and note the FHE scheme, arithmetic representation, hardware platform and supported operations for each relevant accelerator.
- Separate NTT/FFT primitive performance, key-switching performance, bootstrapping and end-to-end application measurements; do not equate their speedups.
- In Section 6, mark which results were reproduced on the authors' testbed and which were imported from the original accelerator papers.
- Audit whether comparisons normalize security parameters, polynomial degrees, hardware generations, memory capacity and timing boundaries.
- Revisit the discussion on on-chip memory, programmability, compiler/scheduler support and scale-up versus scale-out before using the survey to motivate PIM.

## Comparison

The SoK survey provides a literature map, not an independently controlled comparison of [HEAWS](turan-2020-heaws.md), [MemFHE](gupta-2024-memfhe.md) and [FHEmem](zhou-2023-fhemem.md). In particular, MemFHE's RRAM/FHEW model and FHEmem's HBM/CKKS model need to be checked against their original sources rather than treated as one homogeneous PIM category. The older seminar narrative should remain a hypothesis to audit; see the [prior-work archive](../fhe-seminar/provenance.md).

Reading state: Prior-work imported and publication/online text checked; no new complete, version-specific PDF reading or reproduction claimed.
