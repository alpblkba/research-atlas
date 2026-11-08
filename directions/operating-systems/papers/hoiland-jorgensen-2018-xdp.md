---
id: "hoiland-jorgensen-2018-xdp"
title: "The eXpress Data Path: Fast Programmable Packet Processing in the Operating System Kernel"
authors: ["Toke Høiland-Jørgensen", "Jesper Dangaard Brouer", "Daniel Borkmann", "John Fastabend", "Tom Herbert", "David Ahern", "David Miller"]
year: 2018
venue: "CoNEXT 2018, pp. 54-66"
doi: "10.1145/3281411.3281443"
source: "https://doi.org/10.1145/3281411.3281443"
status: "catalogued"
topics: ["operating-systems", "accelerators"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# The eXpress Data Path (XDP)

[Publication DOI](https://doi.org/10.1145/3281411.3281443) · [Direction catalogue](index.md)

## Reading focus

This entry is based on a truncated abstract. Check the full paper before relying on the technical description below.

XDP runs packet programs in the kernel at the driver. I want to trace one packet through that path and compare the protection and tooling it retains with a userspace bypass design.

- Connects industry networking work (data planes, firewalls, load balancers) to OS research.
- A case of a verifier-checked program running in the kernel's fast path.

Reading tier: core for networking and kernel bypass.

## Source record

Source check by agent, 2026-11-06: metadata from OpenAlex; the abstract in the record is truncated.

OpenAlex abstract (truncated in the record): kernel-bypass packet processing is gaining use but removes the operating system's isolation, security and management tooling from the networking path, which motivates XDP.

## Questions for the full paper

- Where in the driver does an XDP program run, and what can it access?
- How does performance compare with DPDK in the paper's setup, and on which NICs?
- Which limits does the eBPF verifier impose on program structure?

## Connections

[Dune](belay-2012-dune.md) · [Forwarding metamorphosis (RMT)](../../accelerators/papers/bosshart-2013-rmt.md) · [Caladan](fried-2020-caladan.md)
