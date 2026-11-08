---
id: "chen-2024-gofetch"
title: "GoFetch: Breaking Constant-Time Cryptographic Implementations Using Data Memory-Dependent Prefetchers"
authors: ["Boru Chen", "Yingchen Wang", "Pradyumna Shome", "Christopher W. Fletcher", "David Kohlbrenner", "Riccardo Paccagnella", "Daniel Genkin"]
year: 2024
venue: "USENIX Security 2024, pp. 1117-1134"
doi: null
source: "https://www.usenix.org/conference/usenixsecurity24/presentation/chen-boru"
status: "catalogued"
topics: ["microarchitectural-security"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# GoFetch

[Source](https://www.usenix.org/conference/usenixsecurity24/presentation/chen-boru) · [Direction catalogue](index.md)

## Reading focus

GoFetch makes the data value itself relevant to prefetching. That is a problem for constant-time code whose security argument accounts for the addresses requested by the program.

- Key extraction from production libraries makes it a clear example of a hardware optimization changing a software security contract.

Reading tier: core for the Apple Silicon thread.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the USENIX presentation page.

USENIX abstract: data memory-dependent prefetchers are a greater threat than previously understood; the authors demonstrate end-to-end attacks on Apple M-series processors and extract keys from constant-time implementations including OpenSSL Diffie-Hellman, Go RSA, CRYSTALS-Kyber and CRYSTALS-Dilithium.

## Questions for the full paper

- Which activation criteria does the prefetcher use, and how were they reverse-engineered?
- Which software or hardware controls disable it, and at what cost?
- Does the threat model require co-location on the same core cluster?

## Connections

[PACMAN](ravichandran-2022-pacman.md) · [Correlation power analysis](../../physical-security/papers/brier-2004-cpa.md) · [FLUSH+RELOAD](yarom-2014-flush-reload.md)
