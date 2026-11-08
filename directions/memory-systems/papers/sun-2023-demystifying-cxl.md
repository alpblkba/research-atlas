---
id: "sun-2023-demystifying-cxl"
title: "Demystifying CXL Memory with Genuine CXL-Ready Systems and Devices"
authors: ["Yan Sun", "Yifan Yuan", "Zeduo Yu", "Reese Kuper", "Chihun Song", "Jinghan Huang", "Houxiang Ji", "Siddharth Agarwal", "Jiaqi Lou", "Ipoom Jeong", "Ren Wang", "Jung Ho Ahn", "Tianyin Xu", "Nam Sung Kim"]
year: 2023
venue: "MICRO 2023, pp. 105-121"
doi: "10.1145/3613424.3614256"
source: "https://arxiv.org/abs/2303.15375v4"
status: "catalogued"
topics: ["memory-systems", "operating-systems"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Demystifying CXL memory

[Publication DOI](https://doi.org/10.1145/3613424.3614256) · [Source](https://arxiv.org/abs/2303.15375v4) · [Direction catalogue](index.md)

## Reading focus

A remote NUMA node is a convenient stand-in for a CXL tier. Measurements on actual CXL devices give me a way to check which latency and bandwidth assumptions that substitution introduces.

- Its page allocation policy (Caption) is an OS mechanism to compare directly with TPP.
- Tianyin Xu, whose SREGym work is already in the vault, is a co-author.

Reading tier: core for the CXL thread.

## Source record

Source check by agent, 2026-11-06: metadata from Crossref; abstract from arXiv v4.

arXiv v4 abstract: the authors evaluate a 4th-generation Intel Xeon system with three CXL memory devices from different vendors, report meaningful differences between emulated and real CXL memory, and propose Caption, a CXL-aware page allocation policy reported to improve bandwidth-intensive applications by up to 24% over the default NUMA policy. Author-reported, on their platform.

## Questions for the full paper

- Which latency and bandwidth characteristics differ from NUMA emulation, and by how much?
- How does Caption choose the share of pages to place on CXL memory?
- Do the three devices differ enough that a conclusion becomes device-specific?

## Connections

[TPP](../../operating-systems/papers/maruf-2023-tpp.md) · [EMT](../../operating-systems/papers/chai-2025-emt.md) · [SREGym](../../systems-reliability/papers/clark-2026-sregym.md)
