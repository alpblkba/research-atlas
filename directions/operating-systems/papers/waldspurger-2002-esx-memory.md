---
id: "waldspurger-2002-esx-memory"
title: "Memory Resource Management in VMware ESX Server"
authors: ["Carl A. Waldspurger"]
year: 2002
venue: "OSDI 2002; ACM SIGOPS Operating Systems Review 36, pp. 181-194"
doi: "10.1145/844128.844146"
source: "https://doi.org/10.1145/844128.844146"
status: "catalogued"
topics: ["operating-systems", "memory-systems"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Memory resource management in VMware ESX Server

[Publication DOI](https://doi.org/10.1145/844128.844146) · [Direction catalogue](index.md)

## Reading focus

ESX combines ballooning, idle-memory taxation and page sharing. I want to distinguish memory the hypervisor can reclaim from memory it can share because the contents match.

- Content-based page sharing later became an attack surface: FLUSH+RELOAD relies on shared pages, and deduplication has been combined with RowHammer, so this paper connects OS memory management to the security directions.

Reading tier: core for the virtualization thread.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: a thin virtualization layer shares hardware among VMs, using ballooning to reclaim memory, an idle-memory tax, and content-based page sharing with I/O page remapping.

## Questions for the full paper

- How does content-based sharing find candidate pages, and what does scanning cost?
- How does ballooning interact with the guest OS's own page replacement?
- Which of these mechanisms are disabled in multi-tenant clouds today for security reasons?

## Connections

[FLUSH+RELOAD](../../microarchitectural-security/papers/yarom-2014-flush-reload.md) · [Formal requirements for virtualizable architectures](popek-1974-virtualizable-architectures.md) · [Flipping bits in memory without accessing them](../../memory-systems/papers/kim-2014-flipping-bits.md)
