---
id: "saileshwar-2021-mirage"
title: "MIRAGE: Mitigating Conflict-Based Cache Attacks with a Practical Fully-Associative Design"
authors: ["Gururaj Saileshwar", "Moinuddin Qureshi"]
year: 2021
venue: "USENIX Security 2021, pp. 1379-1396"
doi: null
source: "https://www.usenix.org/conference/usenixsecurity21/presentation/saileshwar"
status: "catalogued"
topics: ["microarchitectural-security", "computer-architecture"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# MIRAGE

[Source](https://www.usenix.org/conference/usenixsecurity21/presentation/saileshwar) · [Direction catalogue](index.md)

## Reading focus

MIRAGE revisits randomized cache placement after earlier schemes proved vulnerable to eviction-set discovery. What interests me is how closely its design approximates a fully associative cache.

- Shows how a security property is argued for a cache organization and what it costs in storage.
- Saileshwar is also a co-author of GPUHammer and When Mitigations Backfire, so this paper connects the cache-security line with the DRAM-disturbance papers already in the vault.

Reading tier: core.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the USENIX presentation page.

USENIX abstract: MIRAGE selects eviction victims at random from all resident lines using decoupled tag and data stores, extra invalid tags and load-aware skew selection, with reported costs of about 2% slowdown and 17 to 20% more storage than a non-secure cache. Author-reported.

## Questions for the full paper

- What is the security argument (expected time until a set-associative eviction), and under which assumptions?
- Which attacks are out of scope, such as occupancy-based or shared-memory attacks?
- How do the storage and latency costs scale to current server LLC sizes?

## Connections

[RRIP cache replacement](../../computer-architecture/papers/jaleel-2010-rrip.md) · [FLUSH+RELOAD](yarom-2014-flush-reload.md) · [GPUHammer](../../dependable-computing/papers/lin-2025-gpuhammer.md) · [When Mitigations Backfire](../../dependable-computing/papers/woo-2025-when-mitigations-backfire.md)
