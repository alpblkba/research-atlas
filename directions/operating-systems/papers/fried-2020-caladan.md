---
id: "fried-2020-caladan"
title: "Caladan: Mitigating Interference at Microsecond Timescales"
authors: ["Joshua Fried", "Zhenyuan Ruan", "Amy Ousterhout", "Adam Belay"]
year: 2020
venue: "OSDI 2020, pp. 281-297"
doi: null
source: "https://www.usenix.org/conference/osdi20/presentation/fried"
status: "catalogued"
topics: ["operating-systems", "memory-systems"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Caladan

[Source](https://www.usenix.org/conference/osdi20/presentation/fried) · [Direction catalogue](index.md)

## Reading focus

Caladan reallocates resources quickly as load changes. Read it alongside MemGuard to see when that response is fast enough and when a reservation provides a stronger bound.

- Reacts to interference signals at microsecond granularity, a software telemetry loop to compare with hardware telemetry proposals.

Reading tier: core for the interference thread.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the USENIX presentation page.

USENIX abstract: Caladan uses a dedicated scheduling core and a kernel module that bypasses the Linux scheduler to reallocate cores quickly and manage contention, and reports an 11,000x tail-latency improvement over PARTIES when colocating memcached with a best-effort workload. Author-reported, for one comparison setup.

## Questions for the full paper

- Which interference signals are monitored, at what rate, and from which hardware counters?
- Why does fast core reallocation help with memory bandwidth interference that is not core-local?
- How sensitive is the 11,000x figure to the workloads and to the baseline configuration?

## Connections

[MemGuard](../../memory-systems/papers/yun-2013-memguard.md) · [Heracles](../../memory-systems/papers/lo-2015-heracles.md) · [Dune](belay-2012-dune.md)
