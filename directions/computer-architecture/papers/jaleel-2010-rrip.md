---
id: "jaleel-2010-rrip"
title: "High Performance Cache Replacement Using Re-Reference Interval Prediction (RRIP)"
authors: ["Aamer Jaleel", "Kevin B. Theobald", "Simon C. Steely Jr.", "Joel Emer"]
year: 2010
venue: "ISCA 2010, pp. 60-71"
doi: "10.1145/1815961.1815971"
source: "https://doi.org/10.1145/1815961.1815971"
status: "catalogued"
topics: ["computer-architecture", "memory-systems"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# RRIP cache replacement

[Publication DOI](https://doi.org/10.1145/1815961.1815971) · [Direction catalogue](index.md)

## Reading focus

UNVERIFIED against the paper: the technical description below is provisional. The source check covered the bibliographic listing, not the full text or abstract.

When two tasks share a cache, replacement policy decides whose lines survive. RRIP gives me a specific policy to inspect when one task starts slowing down the other.

- RRIP is a low-cost alternative to LRU that resists scans and thrashing, a property that also matters for page-cache thrashing scenarios such as the one contributed to SREGym.
- Cache side-channel and randomized-cache papers often assume an LRU-like policy; knowing RRIP clarifies which eviction assumptions those attacks depend on.

Reading tier: background.

## Source record

Source check by agent, 2026-11-06: metadata from Crossref; the record has no abstract, so the summary below is the agent's and is UNVERIFIED against the paper.

The record carries no abstract. Agent summary: RRIP predicts whether a line will be re-referenced soon or far in the future with a small per-line counter, and inserts new lines with a long predicted interval so that scans do not flush the working set.

## Questions for the full paper

- How do SRRIP and BRRIP differ, and what does set dueling choose between?
- How much per-line state does RRIP need compared with true LRU?
- Does the evaluation include shared-LLC multiprogrammed workloads, and what changes there?

## Connections

[MIRAGE](../../microarchitectural-security/papers/saileshwar-2021-mirage.md) · [Heracles](../../memory-systems/papers/lo-2015-heracles.md) · [The microarchitecture of superscalar processors](smith-1995-superscalar-microarchitecture.md)
