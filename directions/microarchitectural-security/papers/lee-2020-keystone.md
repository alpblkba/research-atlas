---
id: "lee-2020-keystone"
title: "Keystone: An Open Framework for Architecting Trusted Execution Environments"
authors: ["Dayeol Lee", "David Kohlbrenner", "Shweta Shinde", "Krste Asanović", "Dawn Song"]
year: 2020
venue: "EuroSys 2020, pp. 1-16"
doi: "10.1145/3342195.3387532"
source: "https://doi.org/10.1145/3342195.3387532"
status: "catalogued"
topics: ["microarchitectural-security", "operating-systems"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Keystone

[Publication DOI](https://doi.org/10.1145/3342195.3387532) · [Direction catalogue](index.md)

## Reading focus

Keystone builds an enclave around RISC-V physical memory protection. I want to draw exactly where the monitor runs and which component can still grant access to an enclave's memory.

- A RISC-V counterpart to SGX-targeted attacks such as Plundervolt, which helps separate attacks on one TEE implementation from attacks on the TEE idea.
- Relevant to confidential computing on open hardware.

Reading tier: background.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: Keystone is an open-source framework for building customized TEEs on hardware memory isolation, evaluated for security, trusted computing base size and performance.

## Questions for the full paper

- Which RISC-V primitive does it depend on, and what does the security monitor do?
- What is outside the threat model (physical attacks, side channels)?
- How do enclaves rely on the untrusted OS for memory management?

## Connections

[Plundervolt](../../physical-security/papers/murdock-2020-plundervolt.md) · [CHERIoT](amar-2023-cheriot.md) · [ISA semantics in Sail](../../computer-architecture/papers/armstrong-2019-isa-semantics-sail.md)
