---
id: "guajardo-2007-fpga-intrinsic-pufs"
title: "FPGA Intrinsic PUFs and Their Use for IP Protection"
authors: ["Jorge Guajardo", "Sandeep S. Kumar", "Geert-Jan Schrijen", "Pim Tuyls"]
year: 2007
venue: "CHES 2007, pp. 63-80"
doi: "10.1007/978-3-540-74735-2_5"
source: "https://doi.org/10.1007/978-3-540-74735-2_5"
status: "catalogued"
topics: ["physical-security"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# FPGA intrinsic PUFs

[Publication DOI](https://doi.org/10.1007/978-3-540-74735-2_5) · [Direction catalogue](index.md)

## Reading focus

UNVERIFIED against the paper: the technical description below is provisional. The source check covered the bibliographic listing, not the full text or abstract.

The iCE40 experiment reads SRAM at power-up. Guajardo et al. give that observation a PUF context, including the distinction between variation across devices and repeatability on one device.

- Defines how reliability and uniqueness are evaluated and how helper data turns noisy responses into keys.

Reading tier: core, matches existing work.

## Source record

Source check by agent, 2026-11-06: metadata from OpenAlex; the record has no abstract, so the summary below is the agent's and is UNVERIFIED against the paper.

The record carries no abstract. Agent summary: the paper shows that uninitialized SRAM in FPGAs has device-specific power-up states usable as a PUF, characterizes them, and applies them to IP protection with helper-data key extraction.

## Questions for the full paper

- Which FPGA families keep uninitialized SRAM state, and does the iCE40 behave the same way?
- Which metrics are reported, and over how many devices?
- How do temperature and aging change reliability?

## Connections

[OpenRAM](../../computer-architecture/papers/guthaus-2016-openram.md) · [Differential power analysis](kocher-1999-dpa.md)
