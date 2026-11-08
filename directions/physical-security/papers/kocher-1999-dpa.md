---
id: "kocher-1999-dpa"
title: "Differential Power Analysis"
authors: ["Paul Kocher", "Joshua Jaffe", "Benjamin Jun"]
year: 1999
venue: "CRYPTO 1999, pp. 388-397"
doi: "10.1007/3-540-48405-1_25"
source: "https://doi.org/10.1007/3-540-48405-1_25"
status: "catalogued"
topics: ["physical-security"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Differential power analysis

[Publication DOI](https://doi.org/10.1007/3-540-48405-1_25) · [Direction catalogue](index.md)

## Reading focus

UNVERIFIED against the paper: the technical description below is provisional. The source check covered the bibliographic listing, not the full text or abstract.

The CPA experiment in task3 has a predecessor in differential power analysis. I want to compare how each method groups or scores traces under a key hypothesis.

- Defines the difference-of-means test that leakage assessment methods such as TVLA later formalize, and TVLA is the evaluation used in the Meschkov FPGA toolchain paper.

Reading tier: background, short.

## Source record

Source check by agent, 2026-11-06: metadata from OpenAlex; the record has no abstract, so the summary below is the agent's and is UNVERIFIED against the paper.

The record carries no abstract. Agent summary: the paper introduces simple and differential power analysis, recovering keys by relating power consumption to intermediate values that depend on the key.

## Questions for the full paper

- How does the selection function partition traces, and what signal does it isolate?
- Which countermeasures does the paper propose, and which proved insufficient later?
- How does the difference of means compare with CPA's correlation in trace efficiency?

## Connections

[Correlation power analysis](brier-2004-cpa.md) · [Physically secure open-source FPGA and toolchain](meschkov-2025-secure-fpga-toolchain.md)
