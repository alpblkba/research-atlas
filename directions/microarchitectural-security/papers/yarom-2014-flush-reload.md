---
id: "yarom-2014-flush-reload"
title: "FLUSH+RELOAD: A High Resolution, Low Noise, L3 Cache Side-Channel Attack"
authors: ["Yuval Yarom", "Katrina Falkner"]
year: 2014
venue: "USENIX Security 2014, pp. 719-732"
doi: null
source: "https://www.usenix.org/conference/usenixsecurity14/technical-sessions/presentation/yarom"
status: "catalogued"
topics: ["microarchitectural-security"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# FLUSH+RELOAD

[Source](https://www.usenix.org/conference/usenixsecurity14/technical-sessions/presentation/yarom) · [Direction catalogue](index.md)

## Reading focus

Flush+Reload gives an observer a timing signal from a shared cache line. Before reading the later transient-execution papers I want to separate how data reaches the cache from how it is observed.

- Depends on shared pages, which links it to page deduplication in hypervisors.
- Its noise and resolution arguments are the cache-timing analogue of the trace-count arguments in CPA on FPGAs.

Reading tier: core.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the USENIX presentation page.

USENIX abstract: sharing memory pages between mutually distrusting programs leaks information on Intel x86; FLUSH+RELOAD monitors access to shared memory through the last-level cache, and the authors recover about 97% of the private key bits of GnuPG 1.4.13 from a single signing or decryption, across processes and across virtual machines.

## Questions for the full paper

- Which hardware properties are required (inclusive LLC, an unprivileged flush instruction, shared pages)?
- How does the attack change on Arm or Apple cores, where some of these properties differ?
- Which mitigations remove the primitive, and at what cost?

## Connections

[Meltdown](lipp-2018-meltdown.md) · [Memory resource management in VMware ESX Server](../../operating-systems/papers/waldspurger-2002-esx-memory.md) · [Correlation power analysis](../../physical-security/papers/brier-2004-cpa.md)
