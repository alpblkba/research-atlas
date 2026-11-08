---
id: "dixit-2021-sdc-at-scale"
title: "Silent Data Corruptions at Scale"
authors: ["Harish Dattatraya Dixit", "Sneha Pendharkar", "Matt Beadon", "Chris Mason", "Tejasvi Chakravarthy", "Bharath Muthiah", "Sriram Sankar"]
year: 2021
venue: "arXiv preprint"
doi: "10.48550/arXiv.2102.11245"
source: "https://arxiv.org/abs/2102.11245v1"
status: "catalogued"
topics: ["systems-reliability", "dependable-computing"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Silent data corruptions at scale

[arXiv DOI](https://doi.org/10.48550/arXiv.2102.11245) · [Source](https://arxiv.org/abs/2102.11245v1) · [Direction catalogue](index.md)

## Reading focus

The Meta case study follows a CPU fault up to application data loss. I want to see at which layer the first reliable symptom became visible during debugging.

- Read with Cores that don't count to compare two fleets' detection methods.

Reading tier: core, short.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from arXiv v1.

arXiv v1 abstract: hardware faults in CPUs can corrupt data without any error report and surface as software failures; from monitoring hundreds of thousands of machines over more than 18 months, the authors conclude that resilient software design is needed alongside hardware and detection improvements.

## Questions for the full paper

- How was the faulty instruction isolated in the case study?
- Which test method finds SDC-prone parts, and what does it cost in fleet capacity?
- Did a peer-reviewed version follow the arXiv preprint?

## Connections

[Cores that don't count](hochschild-2021-cores-that-dont-count.md) · [Cerberus](../../memory-systems/papers/kim-2026-cerberus.md)
