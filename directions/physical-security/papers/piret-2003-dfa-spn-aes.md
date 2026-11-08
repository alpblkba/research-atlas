---
id: "piret-2003-dfa-spn-aes"
title: "A Differential Fault Attack Technique against SPN Structures, with Application to the AES and Khazad"
authors: ["Gilles Piret", "Jean-Jacques Quisquater"]
year: 2003
venue: "CHES 2003, pp. 77-88"
doi: "10.1007/978-3-540-45238-6_7"
source: "https://doi.org/10.1007/978-3-540-45238-6_7"
status: "catalogued"
topics: ["physical-security"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Piret-Quisquater DFA on AES

[Publication DOI](https://doi.org/10.1007/978-3-540-45238-6_7) · [Direction catalogue](index.md)

## Reading focus

UNVERIFIED against the paper: the technical description below is provisional. The source check covered the bibliographic listing, not the full text or abstract.

My AES note filters faulty ciphertexts for the round-9 byte pattern. Piret and Quisquater explain the recovery step that would use those pairs. The experiment stopped at filtering.

- Explains why a single-byte fault before the last MixColumns spreads to four bytes on one diagonal, the filter used in the task4 scripts.

Reading tier: core, short.

## Source record

Source check by agent, 2026-11-06: metadata from OpenAlex; the record has no abstract, so the summary below is the agent's and is UNVERIFIED against the paper.

The record carries no abstract. Agent summary: a DFA on SPN ciphers that uses byte faults injected before the last MixColumns to recover the AES last-round key from a small number of faulty ciphertexts.

## Questions for the full paper

- How many faulty pairs per diagonal are needed for a unique key, and does that match the two pairs collected in task4?
- What happens when the fault lands in a different round or affects more than one byte?
- How do detection countermeasures (duplication, infection) change the attack?

## Connections

[Differential fault analysis of secret key cryptosystems](biham-1997-dfa.md) · [FPGAhammer](../../dependable-computing/papers/krautter-2018-fpgahammer.md) · [Voltage Drop-based Fault Attacks on FPGAs using Valid Bitstreams](../../dependable-computing/papers/gnad-2017-voltage-drop-fpga.md)
