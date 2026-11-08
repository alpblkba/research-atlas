---
id: "lattner-2004-llvm"
title: "LLVM: A Compilation Framework for Lifelong Program Analysis & Transformation"
authors: ["Chris Lattner", "Vikram Adve"]
year: 2004
venue: "CGO 2004, pp. 75-86"
doi: "10.1109/CGO.2004.1281665"
source: "https://doi.org/10.1109/CGO.2004.1281665"
status: "catalogued"
topics: ["compilers-and-runtimes"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# LLVM

[Publication DOI](https://doi.org/10.1109/CGO.2004.1281665) · [Direction catalogue](index.md)

## Reading focus

LLVM gives clang, Rust and accelerator toolchains a shared intermediate representation. I need to understand what a pass can assume about that IR before looking at PREM's compiler or Alive2.

- Read the IR semantics alongside Alive2 to identify which assumptions a transformation must preserve.

Reading tier: core.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: LLVM is a compiler framework with a typed, SSA-based intermediate representation and mechanisms for analyzing and transforming programs throughout their lifetime.

## Questions for the full paper

- Which IR choices (typed SSA, explicit memory operations) made LLVM reusable beyond C?
- How does the lifelong-optimization idea compare with how LLVM is used today?

## Connections

[MLIR](lattner-2021-mlir.md) · [Alive2](lopes-2021-alive2.md) · [PREM](../../memory-systems/papers/pellizzoni-2011-prem.md)
