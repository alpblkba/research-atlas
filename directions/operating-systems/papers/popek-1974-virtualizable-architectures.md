---
id: "popek-1974-virtualizable-architectures"
title: "Formal Requirements for Virtualizable Third Generation Architectures"
authors: ["Gerald J. Popek", "Robert P. Goldberg"]
year: 1974
venue: "Communications of the ACM 17, pp. 412-421"
doi: "10.1145/361011.361073"
source: "https://doi.org/10.1145/361011.361073"
status: "catalogued"
topics: ["operating-systems", "computer-architecture"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Formal requirements for virtualizable architectures

[Publication DOI](https://doi.org/10.1145/361011.361073) · [Direction catalogue](index.md)

## Reading focus

Popek and Goldberg give a condition for trap-and-emulate virtualization in terms of sensitive and privileged instructions. Dune is easier to reason about once those terms are precise.

- Explains why classic x86 was not virtualizable and why hardware extensions were added, a clean case of an ISA decision constraining OS design.
- A lens for reading the RISC-V privileged architecture and its hypervisor extension.

Reading tier: core, short.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: virtual machines had been built on only a few third-generation systems, so the authors build a formal model of such architectures and derive conditions for testing whether an architecture can support virtual machines.

## Questions for the full paper

- What exactly are the equivalence, resource control and efficiency properties?
- Which x86 instructions violated the condition, and how did hardware virtualization extensions address it?
- Does the RISC-V privileged ISA satisfy the theorem without the H extension?

## Connections

[Dune](belay-2012-dune.md) · [Memory resource management in VMware ESX Server](waldspurger-2002-esx-memory.md)
