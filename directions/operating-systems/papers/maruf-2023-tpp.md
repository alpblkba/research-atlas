---
id: "maruf-2023-tpp"
title: "TPP: Transparent Page Placement for CXL-Enabled Tiered-Memory"
authors: ["Hasan Al Maruf", "Hao Wang", "Abhishek Dhanotia", "Johannes Weiner", "Niket Agarwal", "Pallab Bhattacharya", "Chris Petersen", "Mosharaf Chowdhury", "Shobhit Kanaujia", "Prakash Chauhan"]
year: 2023
venue: "ASPLOS 2023, pp. 742-755"
doi: "10.1145/3582016.3582063"
source: "https://doi.org/10.1145/3582016.3582063"
status: "catalogued"
topics: ["operating-systems", "memory-systems"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# TPP

[Publication DOI](https://doi.org/10.1145/3582016.3582063) · [Direction catalogue](index.md)

## Reading focus

TPP starts with fleet observations about cold memory and uses a kernel policy to move pages between local DRAM and a CXL tier. I want to connect the observed access pattern to the migration decision.

- Pairs with the CXL characterization paper: one measures devices, the other decides placement.
- Page placement under contention is the OS-scale form of the Laxity activation-placement question.

Reading tier: core for the CXL thread.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: the paper examines memory use across Meta's server fleet and shows that colder data can move to slower memory tiers, while performance drops without careful management; TPP is the proposed placement mechanism.

## Questions for the full paper

- How is page temperature measured, and what overhead does sampling add?
- How are promotion and demotion rate-limited to avoid thrashing between tiers?
- Do the results hold on real CXL devices as characterized by Sun et al., or only under emulation?

## Connections

[Demystifying CXL memory](../../memory-systems/papers/sun-2023-demystifying-cxl.md) · [EMT](chai-2025-emt.md) · [Efficient virtual memory for big memory servers (direct segments)](basu-2013-direct-segments.md)
