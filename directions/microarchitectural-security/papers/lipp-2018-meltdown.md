---
id: "lipp-2018-meltdown"
title: "Meltdown: Reading Kernel Memory from User Space"
authors: ["Moritz Lipp", "Michael Schwarz", "Daniel Gruss", "Thomas Prescher", "Werner Haas", "Anders Fogh", "Jann Horn", "Stefan Mangard", "Paul Kocher", "Daniel Genkin", "Yuval Yarom", "Mike Hamburg"]
year: 2018
venue: "USENIX Security 2018, pp. 973-990"
doi: null
source: "https://www.usenix.org/conference/usenixsecurity18/presentation/lipp"
status: "catalogued"
topics: ["microarchitectural-security", "operating-systems"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Meltdown

[Source](https://www.usenix.org/conference/usenixsecurity18/presentation/lipp) · [Direction catalogue](index.md)

## Reading focus

Meltdown exposes a gap between architectural permission checks and transient execution. A load that never commits can still affect state another instruction can measure.

- Changed kernel design (KAISER, later KPTI), so it belongs to the OS direction as much as to architecture.
- A prerequisite for any study of transient leakage on an open OoO core such as BOOM, since the mechanism is defined in terms of the pipeline structures described by Smith and Sohi.

Reading tier: core.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the USENIX presentation page.

USENIX abstract: Meltdown uses side effects of out-of-order execution to let unprivileged programs read kernel memory, and the authors observe that KAISER, originally a KASLR defense, also blocks Meltdown.

## Questions for the full paper

- When exactly is the permission check enforced relative to forwarding the loaded value?
- Which processors were affected, and why were some designs immune?
- What does page-table isolation cost on system-call-heavy workloads?

## Connections

[FLUSH+RELOAD](yarom-2014-flush-reload.md) · [Spectre](kocher-2019-spectre.md) · [The microarchitecture of superscalar processors](../../computer-architecture/papers/smith-1995-superscalar-microarchitecture.md) · [SonicBOOM](../../computer-architecture/papers/zhao-2020-sonicboom.md)
