---
id: "bechtel-2019-cache-dos"
title: "Denial-of-Service Attacks on Shared Cache in Multicore: Analysis and Prevention"
authors: ["Michael Bechtel", "Heechul Yun"]
year: 2019
venue: "RTAS 2019, pp. 357-367"
doi: "10.1109/RTAS.2019.00037"
source: "https://doi.org/10.1109/RTAS.2019.00037"
status: "catalogued"
topics: ["memory-systems", "microarchitectural-security"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Denial-of-service attacks on shared cache

[Publication DOI](https://doi.org/10.1109/RTAS.2019.00037) · [TC 2021 follow-up](https://doi.org/10.1109/TC.2021.3108044) · [Direction catalogue](index.md)

## Reading focus

Even with cache capacity partitioned, a co-runner can still slow another task down. The question I want to carry back to Laxity is which shared resource remains after partitioning.

- Locates the cause in microarchitectural buffers of the non-blocking cache, a reminder that partitioning capacity does not partition every shared structure.
- Proposes an OS-level defense that extends bandwidth regulation, which ties it back to MemGuard.

Reading tier: core for the memory QoS thread.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: attacker tasks can greatly slow a victim on a shared, partitioned cache in multicore systems, traced to the writeback buffer of the non-blocking cache; the authors propose an OS-level defense extending memory bandwidth regulation. A 2021 IEEE Transactions on Computers follow-up exists.

## Questions for the full paper

- On which platforms were the attacks measured, and how large is the worst-case slowdown?
- Which shared buffers (MSHRs, writeback buffer) limit each platform?
- Would a Cortex-M class SoC with banked SRAM behind a bus matrix show an analogous effect?

## Connections

[MemGuard](yun-2013-memguard.md) · [MIRAGE](../../microarchitectural-security/papers/saileshwar-2021-mirage.md) · [PREM](pellizzoni-2011-prem.md)
