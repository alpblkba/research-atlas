---
id: "belay-2012-dune"
title: "Dune: Safe User-level Access to Privileged CPU Features"
authors: ["Adam Belay", "Andrea Bittau", "Ali Mashtizadeh", "David Terei", "David Mazières", "Christos Kozyrakis"]
year: 2012
venue: "OSDI 2012, pp. 335-348"
doi: null
source: "https://www.usenix.org/conference/osdi12/technical-sessions/presentation/belay"
status: "catalogued"
topics: ["operating-systems", "computer-architecture"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Dune

[Source](https://www.usenix.org/conference/osdi12/technical-sessions/presentation/belay) · [Direction catalogue](index.md)

## Reading focus

Dune uses virtualization support to let an ordinary process manage facilities such as page tables. I want to trace which privileges the process gains and which ones the kernel still controls.

- A template for experiments that need page-table control from user space without writing a kernel.
- Leads to later kernel-bypass systems, connecting to XDP and Caladan.

Reading tier: core.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the USENIX presentation page.

USENIX abstract: Dune runs each process inside the CPU's virtualization extensions so it can use privilege rings, page tables and tagged TLBs directly, with a small kernel module and a user-level library; the authors build a sandbox, a privilege separation facility and a garbage collector with it.

## Questions for the full paper

- What does Dune cost on system calls and page faults compared with a normal process?
- Which VT-x features are essential, and could the design work on Arm or RISC-V virtualization extensions?
- Which security boundary does the kernel module still enforce?

## Connections

[Formal requirements for virtualizable architectures](popek-1974-virtualizable-architectures.md) · [The eXpress Data Path (XDP)](hoiland-jorgensen-2018-xdp.md) · [Caladan](fried-2020-caladan.md)
