---
id: "huang-2017-gray-failure"
title: "Gray Failure: The Achilles' Heel of Cloud-Scale Systems"
authors: ["Peng Huang", "Chuanxiong Guo", "Lidong Zhou", "Jacob R. Lorch", "Yingnong Dang", "Murali Chintalapati", "Randolph Yao"]
year: 2017
venue: "HotOS 2017, pp. 150-155"
doi: "10.1145/3102980.3103005"
source: "https://doi.org/10.1145/3102980.3103005"
status: "catalogued"
topics: ["systems-reliability"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Gray failure

[Publication DOI](https://doi.org/10.1145/3102980.3103005) · [Direction catalogue](index.md)

## Reading focus

In a gray failure, a detector can see a healthy component while an application sees degradation. That is exactly the disagreement a recovery benchmark needs to account for when it grades a run.

- A page-cache contention scenario such as the one contributed to SREGym produces latency degradation without a crash, a gray failure in this sense.

Reading tier: core, short.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: cloud availability problems often come from subtle faults rather than complete failures, and monitoring can miss what applications experience; the authors argue for aligning how components perceive failure.

## Questions for the full paper

- How is differential observability defined, and which examples are given?
- Which detection approaches do the authors propose, and is any evaluated?
- How should an SRE agent benchmark score a mitigation for a gray failure?

## Connections

[SREGym](clark-2026-sregym.md) · [STRATUS](chen-2025-stratus.md) · [Heracles](../../memory-systems/papers/lo-2015-heracles.md)
