---
id: "biham-1997-dfa"
title: "Differential Fault Analysis of Secret Key Cryptosystems"
authors: ["Eli Biham", "Adi Shamir"]
year: 1997
venue: "CRYPTO 1997, pp. 513-525"
doi: "10.1007/BFb0052259"
source: "https://doi.org/10.1007/BFb0052259"
status: "catalogued"
topics: ["physical-security"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Differential fault analysis of secret key cryptosystems

[Publication DOI](https://doi.org/10.1007/BFb0052259) · [Direction catalogue](index.md)

## Reading focus

UNVERIFIED against the paper: the technical description below is provisional. The source check covered the bibliographic listing, not the full text or abstract.

My AES fault-analysis note cites Biham and Shamir. The question to bring back to it is which fault assumptions turn an incorrect ciphertext into evidence about a key.

- Separates the fault model (where, when and how many bits change) from the cryptanalysis, the distinction this vault's style contract asks attack notes to keep.

Reading tier: background.

## Source record

Source check by agent, 2026-11-06: metadata from OpenAlex; the record has no abstract, so the summary below is the agent's and is UNVERIFIED against the paper.

The record carries no abstract. Agent summary: introduces differential fault analysis, recovering DES keys by comparing correct and faulty ciphertexts under a transient fault model.

## Questions for the full paper

- Which fault model is assumed, and how realistic is it for voltage-droop faults?
- How many faulty ciphertexts are needed, and how does that change for AES?

## Connections

[Piret-Quisquater DFA on AES](piret-2003-dfa-spn-aes.md) · [FPGAhammer](../../dependable-computing/papers/krautter-2018-fpgahammer.md)
