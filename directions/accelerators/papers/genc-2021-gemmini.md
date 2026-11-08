---
id: "genc-2021-gemmini"
title: "Gemmini: Enabling Systematic Deep-Learning Architecture Evaluation via Full-Stack Integration"
authors: ["Hasan Genc", "Seah Kim", "Alon Amid", "Ameer Haj-Ali", "Vighnesh Iyer", "Pranav Prakash", "Jerry Zhao", "Daniel Grubb", "Harrison Liew", "Howard Mao", "Albert Ou", "Colin Schmidt", "Samuel Steffl", "John Wright", "Ion Stoica", "Jonathan Ragan-Kelley", "Krste Asanović", "Borivoje Nikolić", "Yakun Sophia Shao"]
year: 2021
venue: "DAC 2021, pp. 769-774"
doi: "10.1109/DAC18074.2021.9586216"
source: "https://doi.org/10.1109/DAC18074.2021.9586216"
status: "catalogued"
topics: ["accelerators", "computer-architecture"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Gemmini

[Publication DOI](https://doi.org/10.1109/DAC18074.2021.9586216) · [Direction catalogue](index.md)

## Reading focus

Gemmini puts the matrix engine in a complete SoC. A multiply that looks cheap in isolation can still spend time waiting for the host, translating an address or competing for the cache. Those costs belong in a comparison with rv32i-mla.

- Compare the integrated CPU and accelerator with rv32i-mla under the same workload and memory constraints.

Reading tier: core.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: Gemmini is an open-source generator that builds DNN accelerators inside full SoCs, so that system-level effects such as resource contention and software overhead enter the evaluation.

## Questions for the full paper

- How does Gemmini share the L2 and DRAM with the host core, and which contention is measured?
- How is virtual memory handled for the accelerator's DMA?
- Which parameters (array size, dataflow, scratchpad) does the generator expose?

## Connections

[Chipyard](../../computer-architecture/papers/amid-2020-chipyard.md) · [Timeloop](parashar-2019-timeloop.md) · [Thunderclap](../../operating-systems/papers/markettos-2019-thunderclap.md)
