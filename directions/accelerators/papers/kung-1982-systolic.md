---
id: "kung-1982-systolic"
title: "Why Systolic Architectures?"
authors: ["H. T. Kung"]
year: 1982
venue: "IEEE Computer 15, pp. 37-46"
doi: "10.1109/MC.1982.1653825"
source: "https://doi.org/10.1109/MC.1982.1653825"
status: "catalogued"
topics: ["accelerators", "computer-architecture"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Why systolic architectures?

[Publication DOI](https://doi.org/10.1109/MC.1982.1653825) · [Direction catalogue](index.md)

## Reading focus

A systolic array pays to fetch an operand once and passes it to the next processing element. That's the reuse I want to trace through both the TPU and the MAC array in rv32i-mla.

- Short and conceptual, a good anchor before the TPU and Eyeriss papers.

Reading tier: core, short.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: systolic architectures perform multiple computations per memory access, which can speed up execution.

## Questions for the full paper

- Which algorithm classes map well onto systolic arrays, and which do not?
- How does Kung account for I/O bandwidth against computation, and what does that say about a 4x4 int8 array fed from BRAM?

## Connections

[Tensor Processing Unit](jouppi-2017-tpu.md) · [Eyeriss](chen-2016-eyeriss.md) · [Gemmini](genc-2021-gemmini.md)
