---
id: "zhou-2023-fhemem"
title: "FHEmem: A Processing In-Memory Accelerator for Fully Homomorphic Encryption"
authors: ["Minxuan Zhou", "Yujin Nam", "Pranav Gangwar", "Weihong Xu", "Arpan Dutta", "Kartikeyan Subramanyam", "Chris Wilkerson", "Rosario Cammarota", "Saransh Gupta", "Tajana Rosing"]
year: 2023
venue: "arXiv preprint"
doi: "10.48550/arXiv.2311.16293"
source: "https://arxiv.org/abs/2311.16293v1"
status: "prior-work-imported"
topics: ["accelerators", "memory-systems"]
added: "2026-11-03"
source_checked: "2026-11-03"
read_version: null
---
# FHEmem

[Source: arXiv v1](https://arxiv.org/abs/2311.16293v1) · [FHE comparison](../fhe-data-movement.md)

## What the source and historical work establish

For FHEmem, the obstacle is getting large ciphertexts and wide operands to the arithmetic units often enough to keep them busy. FHEmem proposes processing close to memory together with an end-to-end mapping approach. The preserved seminar slides already explore CKKS workload anatomy, NTT, BConv, key switching, near-mat units, architecture diagrams and evaluation; those are historical draft notes, not claims newly revalidated against the PDF.

## Use the old seminar as an argument to audit

- Find the exact data-movement argument and the working-set assumptions in the paper's Introduction and evaluation.
- Check which FHE schemes, polynomial sizes, number-theoretic transforms and key-switching phases the reported experiments use.
- Distinguish near-mat execution, DRAM-array/internal movement and memory-controller/host communication instead of calling every transfer 'memory bandwidth.'
- Revisit the paper's ablations before claiming a particular part of FHEmem accounts for its overall gains.

## Comparison

[HEAWS](turan-2020-heaws.md) targets FV on an AWS FPGA. It is an architectural comparison point, not an apples-to-apples throughput baseline unless parameters, kernels and measurement boundaries align. Original drafts and caveats: [prior-work archive](../fhe-seminar/provenance.md).

Reading state: Prior-work imported; the 2026 archive does not certify a complete re-reading.
