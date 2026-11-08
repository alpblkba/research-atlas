---
id: "parashar-2019-timeloop"
title: "Timeloop: A Systematic Approach to DNN Accelerator Evaluation"
authors: ["Angshuman Parashar", "Priyanka Raina", "Yakun Sophia Shao", "Yu-Hsin Chen", "Victor A. Ying", "Anurag Mukkara", "Rangharajan Venkatesan", "Brucek Khailany", "Stephen W. Keckler", "Joel Emer"]
year: 2019
venue: "ISPASS 2019, pp. 304-315"
doi: "10.1109/ISPASS.2019.00042"
source: "https://doi.org/10.1109/ISPASS.2019.00042"
status: "catalogued"
topics: ["accelerators"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Timeloop

[Publication DOI](https://doi.org/10.1109/ISPASS.2019.00042) · [Direction catalogue](index.md)

## Reading focus

Two arrays with the same peak MAC rate can run the same layer very differently. Timeloop lets me hold the workload fixed and search the mappings on each architecture.

- A model-based way to locate data-movement bottlenecks in a design like rv32i-mla before building larger arrays.

Reading tier: core for accelerator methodology.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: a framework that models DNN accelerator designs, uses a mapper to schedule operations, and estimates performance and energy to enable fair comparisons.

## Questions for the full paper

- How accurate is the model against the silicon it was validated on?
- How large is the mapping space, and how does the mapper search it?
- Could a 4x4 int8 array with BRAM buffers be described in its specification format?

## Connections

[Eyeriss](chen-2016-eyeriss.md) · [Gemmini](genc-2021-gemmini.md) · [Tensor Processing Unit](jouppi-2017-tpu.md)
