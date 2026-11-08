---
id: "yun-2013-memguard"
title: "MemGuard: Memory Bandwidth Reservation System for Efficient Performance Isolation in Multi-core Platforms"
authors: ["Heechul Yun", "Gang Yao", "Rodolfo Pellizzoni", "Marco Caccamo", "Lui Sha"]
year: 2013
venue: "RTAS 2013, pp. 55-64"
doi: "10.1109/RTAS.2013.6531079"
source: "https://doi.org/10.1109/RTAS.2013.6531079"
status: "catalogued"
topics: ["memory-systems", "operating-systems"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# MemGuard

[Publication DOI](https://doi.org/10.1109/RTAS.2013.6531079) · [TC 2015 extension](https://doi.org/10.1109/TC.2015.2425889) · [Direction catalogue](index.md)

## Reading focus

MemGuard charges memory traffic to cores and regulates their bandwidth. In Laxity the competing requester can be a DMA engine, so the first question is whose budget gets charged.

- Works with performance counters and periodic budgets, so it shows what can be done without new hardware and where that stops (a DMA engine is a bus master, not a core with a budget).
- Use MemGuard and PREM to ground the noisy-neighbor discussion in the Laxity write-up in bandwidth regulation and memory-phase scheduling.
- OpenAlex also lists a 2026 reproduction report on MemGuard's overhead by Chen, Yun and Mancuso (arXiv 2609.04547); not checked beyond the record.

Reading tier: core.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: MemGuard reserves memory bandwidth per core for temporal isolation, reclaims unused reserved bandwidth to improve throughput, and is evaluated with SPEC2006 benchmarks on real hardware. A journal extension appeared in IEEE Transactions on Computers in 2015.

## Questions for the full paper

- Which counter measures bandwidth, at what period, and what does regulation cost in interrupt overhead?
- What happens to masters that are not CPU cores, which is exactly the Laxity aggressor?
- How does the guaranteed bandwidth relate to the assumed worst-case DRAM bandwidth?

## Connections

[PREM](pellizzoni-2011-prem.md) · [Denial-of-service attacks on shared cache](bechtel-2019-cache-dos.md) · [MISE](subramanian-2013-mise.md) · [Caladan](../../operating-systems/papers/fried-2020-caladan.md)
