---
id: "basu-2013-direct-segments"
title: "Efficient Virtual Memory for Big Memory Servers"
authors: ["Arkaprava Basu", "Jayneel Gandhi", "Jichuan Chang", "Mark D. Hill", "Michael M. Swift"]
year: 2013
venue: "ISCA 2013, pp. 237-248"
doi: "10.1145/2485922.2485943"
source: "https://doi.org/10.1145/2485922.2485943"
status: "catalogued"
topics: ["operating-systems", "computer-architecture", "memory-systems"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Efficient virtual memory for big memory servers (direct segments)

[Publication DOI](https://doi.org/10.1145/2485922.2485943) · [Direction catalogue](index.md)

## Reading focus

This entry is based on a truncated abstract. Check the full paper before relying on the technical description below.

A large database may pay for page translation even when most of its memory stays resident. Direct segments ask what a few hardware registers and an OS allocation guarantee can buy for that case.

- Starting point of the virtual-memory thread that EMT and TPP continue.

Reading tier: core.

## Source record

Source check by agent, 2026-11-06: metadata from OpenAlex; the abstract in the record is truncated.

OpenAlex abstract (truncated in the record): large in-memory workloads such as databases, caches and graph analytics lose substantial time to page-based virtual memory overhead even though they rarely need swapping or fine-grained paging.

## Questions for the full paper

- How much TLB-miss overhead is measured, and on which workloads?
- What must the OS guarantee for a direct segment, and what happens under fragmentation?
- How do huge pages compare as a software-only alternative?

## Connections

[EMT](chai-2025-emt.md) · [TPP](maruf-2023-tpp.md) · [The microarchitecture of superscalar processors](../../computer-architecture/papers/smith-1995-superscalar-microarchitecture.md)
