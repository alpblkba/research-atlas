---
id: "fadiheh-2019-upec"
title: "Processor Hardware Security Vulnerabilities and their Detection by Unique Program Execution Checking"
authors: ["Mohammad Rahmani Fadiheh", "Dominik Stoffel", "Clark Barrett", "Subhasish Mitra", "Wolfgang Kunz"]
year: 2019
venue: "DATE 2019, pp. 994-999"
doi: "10.23919/DATE.2019.8715004"
source: "https://doi.org/10.23919/DATE.2019.8715004"
status: "catalogued"
topics: ["microarchitectural-security", "computer-architecture"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Unique program execution checking (UPEC)

[Publication DOI](https://doi.org/10.23919/DATE.2019.8715004) · [Direction catalogue](index.md)

## Reading focus

UPEC checks RTL for cases where secret data changes an observable execution. The useful boundary is the one between the internal difference the checker finds and what an observer can distinguish.

- Argues that such leakage is not limited to high-end processors, which makes it relevant to small in-order cores like rv32i-mla.
- The RPTU Kaiserslautern line that Helium (ISCA 2026) continues with Stanford.

Reading tier: core for secure microarchitecture verification.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: covert-channel leakage, the root cause of Spectre and Meltdown, is not limited to high-end processors; the authors propose Unique Program Execution Checking, a formal method that detects and locates such vulnerabilities, including unknown ones.

## Questions for the full paper

- How is the property formulated, and what does the two-instance model look like?
- What scalability limits apply, and on which cores was it run?
- Which vulnerability was found in a simple in-order core, and why did it exist?

## Connections

[Helium](archer-2026-helium.md) · [Speculative taint tracking (STT)](yu-2019-stt.md) · [ISA semantics in Sail](../../computer-architecture/papers/armstrong-2019-isa-semantics-sail.md)
