---
id: "chen-2016-eyeriss"
title: "Eyeriss: A Spatial Architecture for Energy-Efficient Dataflow for Convolutional Neural Networks"
authors: ["Yu-Hsin Chen", "Joel Emer", "Vivienne Sze"]
year: 2016
venue: "ISCA 2016, pp. 367-379"
doi: "10.1109/ISCA.2016.40"
source: "https://doi.org/10.1109/ISCA.2016.40"
status: "catalogued"
topics: ["accelerators", "memory-systems"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Eyeriss

[Publication DOI](https://doi.org/10.1109/ISCA.2016.40) · [Direction catalogue](index.md)

## Reading focus

In Eyeriss, the choice of dataflow determines which operand stays put and which one has to travel. I want to compare weight-, output- and row-stationary mappings by counting those transfers for the same layer.

- The same lens as the FHE data-movement note: energy is dominated by where data moves rather than by arithmetic.

Reading tier: core.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: a row-stationary dataflow reduces data movement by reusing filter weights, input activations and partial sums, validated on AlexNet and a fabricated chip.

## Questions for the full paper

- How is energy per access modeled at each level of the storage hierarchy?
- How does row stationary compare with the other dataflows under the same storage budget?
- Which parts of the analysis apply to a tiny 4x4 array?

## Connections

[Timeloop](parashar-2019-timeloop.md) · [Why systolic architectures?](kung-1982-systolic.md) · [FHE data movement](../fhe-data-movement.md)
