---
id: "lattuada-2024-verus"
title: "Verus: A Practical Foundation for Systems Verification"
authors: ["Andrea Lattuada", "Travis Hance", "Jay Bosamiya", "Matthias Brun", "Chanhee Cho", "Hayley LeBlanc", "Pranav Srinivasan", "Reto Achermann", "Tej Chajed", "Chris Hawblitzel", "Jon Howell", "Jacob R. Lorch", "Oded Padon", "Bryan Parno"]
year: 2024
venue: "SOSP 2024, pp. 438-454"
doi: "10.1145/3694715.3695952"
source: "https://doi.org/10.1145/3694715.3695952"
status: "catalogued"
topics: ["operating-systems", "compilers-and-runtimes"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Verus

[Publication DOI](https://doi.org/10.1145/3694715.3695952) · [Direction catalogue](index.md)

## Reading focus

This entry is based on a truncated abstract. Check the full paper before relying on the technical description below.

Verus uses an SMT solver to verify Rust systems code. The paper gives me a place to check what the programmer has to specify and what the solver can discharge.

- Gives the comparison point to seL4's interactive proofs: what is automated, and what still needs manual proof effort.
- Relevant to verified firmware or drivers where Rust is an option.

Reading tier: core for the verification thread.

## Source record

Source check by agent, 2026-11-06: metadata from OpenAlex; the abstract in the record is truncated.

OpenAlex abstract (truncated in the record): formal verification can catch bugs before software ships, but earlier projects required heavy effort, custom logics or limited automation, motivating a more practical foundation.

## Questions for the full paper

- Which systems were verified in the paper, and what proof-to-code ratios are reported?
- How does Verus treat unsafe Rust, concurrency and hardware interaction?
- Where does the SMT-based approach fail or slow down?

## Connections

[seL4](klein-2009-sel4.md) · [Alive2](../../compilers-and-runtimes/papers/lopes-2021-alive2.md) · [ISA semantics in Sail](../../computer-architecture/papers/armstrong-2019-isa-semantics-sail.md)
