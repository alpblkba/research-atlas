---
id: "lo-2015-heracles"
title: "Heracles: Improving Resource Efficiency at Scale"
authors: ["David Lo", "Liqun Cheng", "Rama Govindaraju", "Parthasarathy Ranganathan", "Christos Kozyrakis"]
year: 2015
venue: "ISCA 2015"
doi: "10.1145/2749469.2749475"
source: "https://doi.org/10.1145/2749469.2749475"
status: "catalogued"
topics: ["memory-systems", "systems-reliability"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Heracles

[Publication DOI](https://doi.org/10.1145/2749469.2749475) · [Direction catalogue](index.md)

## Reading focus

UNVERIFIED against the paper: the technical description below is provisional. The source check covered the bibliographic listing, not the full text or abstract.

Heracles puts a latency-sensitive service next to best-effort work. Compared with Laxity, the controller has more places to intervene: cores, cache, memory bandwidth, power and the network.

- Shows hardware isolation features driven by a feedback controller, which is the system that surrounds any hardware telemetry mechanism.
- Connects the MCU-scale Laxity measurement to the cloud-scale interference injected in SREGym scenarios.

Reading tier: core.

## Source record

Source check by agent, 2026-11-06: metadata from Crossref; the record has no abstract, so the summary below is the agent's and is UNVERIFIED against the paper.

The Crossref record lists the title as "Heracles" with the subtitle separate and has no abstract. Agent summary: Heracles is a feedback controller that lets best-effort tasks share servers with latency-critical services while keeping their tail latency within its target.

## Questions for the full paper

- Which isolation mechanisms are used, and which resource was hardest to isolate?
- How is memory bandwidth measured and controlled without per-thread hardware counters?
- Which utilization gain is reported, and on which services?

## Connections

[Caladan](../../operating-systems/papers/fried-2020-caladan.md) · [MISE](subramanian-2013-mise.md) · [SREGym](../../systems-reliability/papers/clark-2026-sregym.md) · [Gray failure](../../systems-reliability/papers/huang-2017-gray-failure.md)
