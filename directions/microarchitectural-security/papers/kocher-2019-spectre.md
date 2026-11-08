---
id: "kocher-2019-spectre"
title: "Spectre Attacks: Exploiting Speculative Execution"
authors: ["Paul Kocher", "Jann Horn", "Anders Fogh", "Daniel Genkin", "Daniel Gruss", "Werner Haas", "Mike Hamburg", "Moritz Lipp", "Stefan Mangard", "Thomas Prescher", "Michael Schwarz", "Yuval Yarom"]
year: 2019
venue: "IEEE S&P 2019, pp. 1-19"
doi: "10.1109/SP.2019.00002"
source: "https://doi.org/10.1109/SP.2019.00002"
status: "catalogued"
topics: ["microarchitectural-security", "computer-architecture"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Spectre

[Publication DOI](https://doi.org/10.1109/SP.2019.00002) · [Direction catalogue](index.md)

## Reading focus

A bad branch prediction normally gets squashed. Spectre asks which effects of the transient instructions remain observable afterward, a question I can trace from predictor state through the cache.

- Its call for a shared model of what speculation may leak is the problem statement that STT, UPEC and Helium respond to.

Reading tier: core.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: practical attacks induce processors to leak data through speculative execution, and the authors argue that hardware and ISA designers need a shared model of what speculative computation may leak.

## Questions for the full paper

- Which variants use the conditional branch predictor and which the BTB, and what attacker control does each need?
- Why is Spectre harder to fix in hardware than Meltdown?
- What would a contract between the ISA and software about speculation look like?

## Connections

[TAGE branch prediction](../../computer-architecture/papers/seznec-2006-tage.md) · [Meltdown](lipp-2018-meltdown.md) · [Speculative taint tracking (STT)](yu-2019-stt.md) · [Unique program execution checking (UPEC)](fadiheh-2019-upec.md)
