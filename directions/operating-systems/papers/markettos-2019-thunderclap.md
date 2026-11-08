---
id: "markettos-2019-thunderclap"
title: "Thunderclap: Exploring Vulnerabilities in Operating System IOMMU Protection via DMA from Untrustworthy Peripherals"
authors: ["A. Theodore Markettos", "Colin Rothwell", "Brett F. Gutstein", "Allison Pearce", "Peter G. Neumann", "Simon W. Moore", "Robert N. M. Watson"]
year: 2019
venue: "NDSS 2019"
doi: "10.14722/ndss.2019.23194"
source: "https://doi.org/10.14722/ndss.2019.23194"
status: "catalogued"
topics: ["operating-systems", "microarchitectural-security"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Thunderclap

[Publication DOI](https://doi.org/10.14722/ndss.2019.23194) · [Direction catalogue](index.md)

## Reading focus

Laxity's DMA engine competes for bandwidth. Thunderclap changes the assumption that the device is trusted and asks which memory the OS actually exposes through the IOMMU.

- Impersonates peripherals with an FPGA-based platform, a technique close to the board tooling in fpgatest.
- A protection boundary that fails because of how the OS uses the hardware rather than because of the hardware alone.

Reading tier: core for the I/O and DMA thread.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: peripherals using DMA can bypass operating system IOMMU protections in several ways; the authors describe an FPGA-based platform used to demonstrate the weaknesses, which vendors then worked to fix.

## Questions for the full paper

- Which OS IOMMU usage patterns (shared mappings, deferred invalidation) create the exposure?
- What does the FPGA platform emulate, and over which interfaces?
- How do the findings change for SoC-internal DMA engines rather than external peripherals?

## Connections

[CHERIoT](../../microarchitectural-security/papers/amar-2023-cheriot.md) · [MemGuard](../../memory-systems/papers/yun-2013-memguard.md) · [Gemmini](../../accelerators/papers/genc-2021-gemmini.md)
