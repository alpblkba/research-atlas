---
id: "jouppi-2017-tpu"
title: "In-Datacenter Performance Analysis of a Tensor Processing Unit"
authors: ["Norman P. Jouppi", "Cliff Young", "Nishant Patil", "David Patterson", "et al. (76 authors in the OpenAlex record)"]
year: 2017
venue: "ISCA 2017, pp. 1-12"
doi: "10.1145/3079856.3080246"
source: "https://doi.org/10.1145/3079856.3080246"
status: "catalogued"
topics: ["accelerators"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Tensor Processing Unit

[Publication DOI](https://doi.org/10.1145/3079856.3080246) · [Direction catalogue](index.md)

## Reading focus

The TPU has plenty of INT8 MACs. The roofline plots tell me which production workloads could actually keep them busy and which ran out of bandwidth first.

- Uses the same quantized int8 data type as the rv32i-mla accelerator, at datacenter scale.

Reading tier: core.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: the paper evaluates Google's TPU inference accelerator and reports it as much faster and more energy-efficient than contemporary CPUs and GPUs on neural-network workloads.

## Questions for the full paper

- Which workloads are memory-bound on the TPU, and why does the roofline place them there?
- How large is the systolic array, and how is weight loading overlapped with compute?
- Which design decisions follow from deployment constraints such as PCIe attachment and latency targets?

## Connections

[Why systolic architectures?](kung-1982-systolic.md) · [Eyeriss](chen-2016-eyeriss.md) · [Timeloop](parashar-2019-timeloop.md)
