---
id: "subramanian-2013-mise"
title: "MISE: Providing Performance Predictability and Improving Fairness in Shared Main Memory Systems"
authors: ["Lavanya Subramanian", "Vivek Seshadri", "Yoongu Kim", "Ben Jaiyen", "Onur Mutlu"]
year: 2013
venue: "HPCA 2013, pp. 639-650"
doi: "10.1109/HPCA.2013.6522356"
source: "https://doi.org/10.1109/HPCA.2013.6522356"
status: "catalogued"
topics: ["memory-systems"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# MISE

[Publication DOI](https://doi.org/10.1109/HPCA.2013.6522356) · [Direction catalogue](index.md)

## Reading focus

MISE estimates slowdown from the rate at which the controller serves an application's requests. I want to know what the controller must observe to distinguish interference from a change in demand.

- Laxity measures placement-dependent slowdown under GPDMA contention offline; MISE models how a controller could estimate such slowdown at runtime.
- Links scheduling in the memory controller to QoS guarantees, the same knob that MemGuard regulates from software.

Reading tier: core for the memory QoS thread.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: applications sharing main memory slow each other unevenly; the authors propose a simple model that estimates each application's slowdown from how quickly its memory requests are served, and use it to build QoS and fairness schedulers.

## Questions for the full paper

- How is the alone request service rate estimated while the application runs shared?
- How large is the model's error, and for which workload classes does it break down?
- Which counters would the model need on a real controller or on an SoC bus matrix?

## Connections

[Memory access scheduling](rixner-2000-memory-access-scheduling.md) · [MemGuard](yun-2013-memguard.md) · [Heracles](lo-2015-heracles.md)
