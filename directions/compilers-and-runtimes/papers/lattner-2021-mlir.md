---
id: "lattner-2021-mlir"
title: "MLIR: Scaling Compiler Infrastructure for Domain Specific Computation"
authors: ["Chris Lattner", "Mehdi Amini", "Uday Bondhugula", "Albert Cohen", "Andy Davis", "Jacques Pienaar", "River Riddle", "Tatiana Shpeisman", "Nicolas Vasilache", "Oleksandr Zinenko"]
year: 2021
venue: "CGO 2021, pp. 2-14"
doi: "10.1109/CGO51591.2021.9370308"
source: "https://doi.org/10.1109/CGO51591.2021.9370308"
status: "catalogued"
topics: ["compilers-and-runtimes", "accelerators"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# MLIR

[Publication DOI](https://doi.org/10.1109/CGO51591.2021.9370308) · [Direction catalogue](index.md)

## Reading focus

In MLIR a compiler can keep tensor operations intact until it has enough target information to lower them. The question for a custom accelerator is which decision belongs at each level.

- A route to compiler support for a small custom accelerator: describe its operations as a dialect instead of writing a compiler from scratch.

Reading tier: background.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: MLIR is a reusable, extensible compiler infrastructure meant to reduce the cost of building domain-specific compilers and to connect existing compilers; the paper covers design, semantics and evaluation.

## Questions for the full paper

- What is a dialect, and how do progressive lowering and verification interact?
- Which accelerator projects use MLIR, and what did it save them?

## Connections

[LLVM](lattner-2004-llvm.md) · [Gemmini](../../accelerators/papers/genc-2021-gemmini.md) · [Forwarding metamorphosis (RMT)](../../accelerators/papers/bosshart-2013-rmt.md)
