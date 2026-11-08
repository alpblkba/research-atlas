---
id: "pellizzoni-2011-prem"
title: "A Predictable Execution Model for COTS-Based Embedded Systems"
authors: ["Rodolfo Pellizzoni", "Emiliano Betti", "Stanley Bak", "Gang Yao", "John Criswell", "Marco Caccamo", "Russell Kegley"]
year: 2011
venue: "RTAS 2011, pp. 269-279"
doi: "10.1109/RTAS.2011.33"
source: "https://doi.org/10.1109/RTAS.2011.33"
status: "catalogued"
topics: ["memory-systems", "compilers-and-runtimes"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# PREM

[Publication DOI](https://doi.org/10.1109/RTAS.2011.33) · [Direction catalogue](index.md)

## Reading focus

PREM divides a task into memory and compute phases. If memory requests can be scheduled ahead of time, some of the interference Laxity measures becomes a scheduling decision.

- Produces the phases with a modified LLVM compiler, which links the memory QoS thread to compilers and runtimes.
- Argues for bounded interference rather than throughput, which complements MemGuard's regulation.

Reading tier: core.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: real-time systems built from COTS components suffer unpredictable delays from shared resources; the authors propose keeping each shared resource below saturation, introduce the PREM model and validate it on a COTS testbed using a modified LLVM compiler.

## Questions for the full paper

- What must a task look like to be split into predictable intervals, and who does the splitting?
- How are DMA-capable peripherals handled in the model?
- How much average-case performance is given up to obtain the worst-case bound?

## Connections

[MemGuard](yun-2013-memguard.md) · [TensorFlow Lite Micro](../../compilers-and-runtimes/papers/david-2021-tflm.md) · [LLVM](../../compilers-and-runtimes/papers/lattner-2004-llvm.md)
