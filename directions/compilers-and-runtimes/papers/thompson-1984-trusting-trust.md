---
id: "thompson-1984-trusting-trust"
title: "Reflections on Trusting Trust"
authors: ["Ken Thompson"]
year: 1984
venue: "Communications of the ACM 27(8), pp. 761-763"
doi: "10.1145/358198.358210"
source: "https://doi.org/10.1145/358198.358210"
status: "catalogued"
topics: ["compilers-and-runtimes"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Reflections on trusting trust

[Publication DOI](https://doi.org/10.1145/358198.358210) · [Direction catalogue](index.md)

## Reading focus

A compromised compiler can compile its own behavior into its successor even when its source looks clean. That leaves a trust question at the binary I actually run.

- The same question applies to hardware toolchains, where a bitstream or netlist is also a compiled artifact.

Reading tier: core, three pages.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: the essay asks how far one can trust a claim that a program is free of Trojan horses, and argues that the question matters most to the people who write software.

## Questions for the full paper

- Which step makes the attack self-perpetuating?
- How do reproducible builds and diverse double-compiling address it?
- What is the equivalent attack for synthesis and place-and-route tools?

## Connections

[Reproducible builds](lamb-2022-reproducible-builds.md) · [Nix](dolstra-2004-nix.md) · [Physically secure open-source FPGA and toolchain](../../physical-security/papers/meschkov-2025-secure-fpga-toolchain.md)
