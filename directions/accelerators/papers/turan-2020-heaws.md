---
id: "turan-2020-heaws"
title: "HEAWS: An Accelerator for Homomorphic Encryption on the Amazon AWS FPGA"
authors: ["Furkan Turan", "Sujoy Sinha Roy", "Ingrid Verbauwhede"]
year: 2020
venue: "IEEE Transactions on Computers 69(8), 1185–1196"
doi: "10.1109/TC.2020.2988765"
source: "https://www.esat.kuleuven.be/cosic/publications/article-3184.pdf"
status: "prior-work-imported"
topics: ["accelerators"]
added: "2026-11-03"
source_checked: "2026-11-03"
read_version: null
---
# HEAWS

[Original author PDF](https://www.esat.kuleuven.be/cosic/publications/article-3184.pdf) · [FHE comparison](../fhe-data-movement.md)

## Abstract-level architecture

HEAWS runs FV polynomial arithmetic on parallel coprocessors in an AWS FPGA. Its paper abstract and opening pages describe multiple coprocessors, on-chip polynomial storage, 512-bit XDMA host/FPGA communication and explicit optimization of off-chip transfers. The paper reports application and operation-level performance, but headline throughput without scheme/parameter context is not comparable to FHEmem.

## What to extract if revisiting the paper

- Number and role of replicated coprocessors, FPGA resource use and memory mapping.
- How NTT/data access and the host-device interface are scheduled; where transfer overhead enters the timing boundary.
- Whether the reported operation rate is for FV parameters equivalent to any workload cited in the preserved FHEmem seminar.
- How much of the end-to-end application speedup depends on the platform, not only the arithmetic datapath.

The previous seminar materials mention HEAWS as a compute-centric comparison point. See [historical files](../fhe-seminar/provenance.md) and the source-reconciliation exercise.

Reading state: Prior-work imported; no fresh full-paper review claimed.
