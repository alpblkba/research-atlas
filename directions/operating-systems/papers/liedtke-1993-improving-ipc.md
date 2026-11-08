---
id: "liedtke-1993-improving-ipc"
title: "Improving IPC by Kernel Design"
authors: ["Jochen Liedtke"]
year: 1993
venue: "SOSP 1993, pp. 175-188"
doi: "10.1145/168619.168633"
source: "https://doi.org/10.1145/168619.168633"
status: "catalogued"
topics: ["operating-systems"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Improving IPC by kernel design

[Publication DOI](https://doi.org/10.1145/168619.168633) · [Direction catalogue](index.md)

## Reading focus

In a microkernel, crossing a protection boundary is ordinary work. Liedtke designs L4 around the cost of that IPC path, which makes the individual steps worth counting.

- Relevant to inter-processor communication and mailbox-based firmware transports, where the same questions arise: register-only messages, avoiding copies, and scheduling on send.
- Background for seL4, which inherits the L4 design.

Reading tier: core for the operating-systems direction.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: fast interprocess communication is critical for microkernels, and careful kernel design can make it much faster than in existing systems.

## Questions for the full paper

- Which techniques give the largest gains (direct process switch, register messages, lazy scheduling, address-space handling)?
- Which of them depend on 1993 x86 details, and which carry over to Arm or RISC-V?
- How would the same principles apply to a hardware mailbox between two cores?

## Connections

[seL4](klein-2009-sel4.md) · [The Multikernel](baumann-2009-multikernel.md)
