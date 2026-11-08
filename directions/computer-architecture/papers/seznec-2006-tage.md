---
id: "seznec-2006-tage"
title: "A case for (partially) TAgged GEometric history length branch prediction"
authors: ["André Seznec", "Pierre Michaud"]
year: 2006
venue: "Journal of Instruction-Level Parallelism 8 (February 2006)"
doi: null
source: "http://www.jilp.org/vol8/v8paper1.pdf"
status: "catalogued"
topics: ["computer-architecture"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# TAGE branch prediction

[Source](http://www.jilp.org/vol8/v8paper1.pdf) · [JILP volume 8 index](https://jilp.org/vol8/index.html) · [Direction catalogue](index.md)

## Reading focus

UNVERIFIED against the paper: the technical description below is provisional. The source check covered the bibliographic listing, not the full text or abstract.

SonicBOOM uses TAGE in its fetch unit. The first comparison I want is with the two-bit predictor in rv32i-mla: what history can each predictor use when the same branch comes around again?

- Compare storage, indexing and update logic at a fixed predictor budget.
- Branch predictors are shared microarchitectural state, which is why they reappear as Spectre training primitives and as side channels.

Reading tier: core for the computer-architecture direction.

## Source record

Source check by agent, 2026-11-06: listing from the JILP volume 8 index; abstract not checked, summary UNVERIFIED.

The listing (title, authors, February 2006) was checked on the JILP volume 8 index. The PDF text did not extract cleanly, so the abstract is not checked. Agent summary: TAGE combines a base predictor with several tagged tables indexed by global history lengths that grow geometrically, and predicts with the longest matching history.

## Questions for the full paper

- How are allocation on misprediction and the usefulness counters defined, and what happens to accuracy when they are simplified?
- What storage budget sits behind the reported accuracy, and how does it compare with gshare or a perceptron predictor at the same budget?
- Which parts of the index and tag computation would be expensive in an FPGA soft core?

## Connections

[The microarchitecture of superscalar processors](smith-1995-superscalar-microarchitecture.md) · [SonicBOOM](zhao-2020-sonicboom.md) · [Spectre](../../microarchitectural-security/papers/kocher-2019-spectre.md)
