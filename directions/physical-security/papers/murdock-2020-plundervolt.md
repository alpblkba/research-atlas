---
id: "murdock-2020-plundervolt"
title: "Plundervolt: Software-based Fault Injection Attacks against Intel SGX"
authors: ["Kit Murdock", "David Oswald", "Flavio D. Garcia", "Jo Van Bulck", "Daniel Gruss", "Frank Piessens"]
year: 2020
venue: "IEEE S&P 2020, pp. 1466-1482"
doi: "10.1109/SP40000.2020.00057"
source: "https://doi.org/10.1109/SP40000.2020.00057"
status: "catalogued"
topics: ["physical-security", "microarchitectural-security"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Plundervolt

[Publication DOI](https://doi.org/10.1109/SP40000.2020.00057) · [Direction catalogue](index.md)

## Reading focus

Plundervolt uses software-controlled undervolting to induce faults in SGX computations on x86. Compare it with CLKSCREW on the privilege required and the computation affected.

- Followed by a vendor fix at the microcode and interface level, a case study of how a physical-fault vulnerability is mitigated on a deployed platform.

Reading tier: core.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: software-controlled voltage and frequency scaling can induce predictable faults in SGX enclave computations, enabling key recovery and memory-safety violations, and the authors argue that a fix is not trivial.

## Questions for the full paper

- Which instructions fault first under undervolting, and why?
- What did the vendor mitigation change, and does it remove the attack class or only this interface?
- How does the fault model compare with the AES round-9 byte fault used in task4?

## Connections

[CLKSCREW](tang-2017-clkscrew.md) · [Keystone](../../microarchitectural-security/papers/lee-2020-keystone.md) · [Piret-Quisquater DFA on AES](piret-2003-dfa-spn-aes.md)
