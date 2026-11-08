---
id: "baumann-2009-multikernel"
title: "The Multikernel: A New OS Architecture for Scalable Multicore Systems"
authors: ["Andrew Baumann", "Paul Barham", "Pierre-Évariste Dagand", "Tim Harris", "Rebecca Isaacs", "Simon Peter", "Timothy Roscoe", "Adrian Schüpbach", "Akhilesh Singhania"]
year: 2009
venue: "SOSP 2009, pp. 29-44"
doi: "10.1145/1629575.1629579"
source: "https://doi.org/10.1145/1629575.1629579"
status: "catalogued"
topics: ["operating-systems", "computer-architecture"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# The Multikernel

[Publication DOI](https://doi.org/10.1145/1629575.1629579) · [Direction catalogue](index.md)

## Reading focus

This entry is based on a truncated abstract. Check the full paper before relying on the technical description below.

The multikernel treats cores as nodes and sends messages to coordinate kernel state. The comparison I care about is when communicating explicitly costs less than keeping shared state coherent.

- Relevant to heterogeneous SoCs whose cores and coprocessors do not share coherent memory.
- From the ETH Systems Group, which later built Enzian.

Reading tier: core.

## Source record

Source check by agent, 2026-11-06: metadata from OpenAlex; the abstract in the record is truncated.

OpenAlex abstract (truncated in the record after the motivation): increasingly diverse hardware and workloads make it impractical to tune one OS structure for every case, which motivates rethinking OS structure.

## Questions for the full paper

- How is replicated state kept consistent, and at what cost compared with shared-memory locking?
- Which measurements show message passing ahead of shared memory, and on which hardware?
- Which Barrelfish ideas survived into later systems?

## Connections

[Improving IPC by kernel design](liedtke-1993-improving-ipc.md) · [Shared memory consistency models](../../computer-architecture/papers/adve-1996-memory-consistency-tutorial.md) · [Enzian](../../computer-architecture/papers/cock-2022-enzian.md)
