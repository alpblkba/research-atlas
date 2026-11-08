---
id: "gupta-2024-memfhe"
title: "MemFHE: End-to-End Computing with Fully Homomorphic Encryption in Memory"
authors: ["Saransh Gupta", "Rosario Cammarota", "Tajana Šimunić Rosing"]
year: 2024
venue: "ACM Transactions on Embedded Computing Systems 23(2)"
doi: "10.1145/3569955"
source: "https://arxiv.org/abs/2204.12557"
status: "prior-work-imported"
topics: ["accelerators", "memory-systems"]
added: "2026-11-03"
source_checked: "2026-11-03"
read_version: null
---
# MemFHE

[Source: arXiv (first submitted 2022)](https://arxiv.org/abs/2204.12557) · [Published article](https://doi.org/10.1145/3569955) · [FHE comparison](../fhe-data-movement.md)

## Mechanism and evidence

MemFHE divides FHEW/Ring-GSW-style work between two RRAM processing-in-memory units. It separates a client-PIM for encryption and decryption from a server-PIM for evaluating encrypted functions. The server uses a deeply pipelined flow involving bootstrapping, key switching and modulus switching, with alternative AP and GINX accumulation procedures. Its central architectural argument is that in-memory execution and parallelism can reduce the cost of moving expanded ciphertexts and large cryptographic keys. The reported performance is based on a cycle-accurate architecture simulator and HSPICE-derived operation models, not measured accelerator silicon. Section 9 reports results for multiple security parameters and compares specific arithmetic and neural-network workloads with CPU, GPU and TDNN baselines.

## Details to check

- Trace the complete client/server dataflow and distinguish ciphertext transfer across the network from data movement inside the memory-based accelerator.
- Map the stages of bootstrapping, including accumulation, NTT/iNTT, key switching and modulus switching, to the RRAM memory blocks and pipeline boundaries.
- Check the AP versus GINX trade-off and how cryptographic keys, pipeline stages and available memory determine throughput and capacity requirements.
- Separate single-operation latency from saturated-pipeline throughput; check which reported gains depend on batches of independent operations.
- Record the precise security parameters, memory budgets, CPU/GPU baselines and measurement boundaries behind the arithmetic and neural-network speedups.

## Comparison

[MemFHE](https://arxiv.org/abs/2204.12557) is RRAM-based and focuses on FHEW/Ring-GSW-style workloads; [FHEmem](zhou-2023-fhemem.md) is an HBM/DRAM near-mat proposal centered on CKKS. [HEAWS](turan-2020-heaws.md) uses FV on an AWS FPGA. Their speedups are not interchangeable without matching schemes, parameters, operations, memory assumptions and baseline definitions. The earlier seminar material is historical context, not an independently replicated benchmark; see the [prior-work archive](../fhe-seminar/provenance.md).

Reading state: Prior-work imported and uploaded source inspected for architecture and evaluation boundaries; this note does not certify a complete independent re-reading or reproduction.
