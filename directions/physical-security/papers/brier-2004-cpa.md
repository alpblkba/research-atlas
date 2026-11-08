---
id: "brier-2004-cpa"
title: "Correlation Power Analysis with a Leakage Model"
authors: ["Éric Brier", "Christophe Clavier", "Francis Olivier"]
year: 2004
venue: "CHES 2004, pp. 16-29"
doi: "10.1007/978-3-540-28632-5_2"
source: "https://doi.org/10.1007/978-3-540-28632-5_2"
status: "catalogued"
topics: ["physical-security"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Correlation power analysis

[Publication DOI](https://doi.org/10.1007/978-3-540-28632-5_2) · [Direction catalogue](index.md)

## Reading focus

UNVERIFIED against the paper: the technical description below is provisional. The source check covered the bibliographic listing, not the full text or abstract.

The AES lab uses correlation power analysis with an on-chip FPGA sensor. FIPS 197 specifies AES, but this paper is the reference I need for the leakage model behind the correlation.

- Introduces the Hamming distance leakage model with correlation as the distinguisher; task3 correlates against a bitwise leakage model on the last-round inverse S-box instead, so this paper is the reference for why the choice of model matters.

Reading tier: core.

## Source record

Source check by agent, 2026-11-06: metadata from OpenAlex; the record has no abstract, so the summary below is the agent's and is UNVERIFIED against the paper.

The record carries no abstract. Agent summary: the paper models power consumption as linear in the Hamming distance of a register transition and uses the correlation coefficient between predicted and measured leakage to recover keys.

## Questions for the full paper

- Why Hamming distance rather than Hamming weight, and when does the choice matter for an FPGA register?
- How does the number of traces needed scale with signal-to-noise ratio?
- How does the leakage model apply to a delay-based on-chip sensor instead of a shunt resistor?

## Connections

[Differential power analysis](kocher-1999-dpa.md) · [Sensing nanosecond-scale voltage attacks in FPGAs](zick-2013-sensing-voltage-transients.md) · [An Inside Job](../../dependable-computing/papers/schellenberg-2018-inside-job.md)
