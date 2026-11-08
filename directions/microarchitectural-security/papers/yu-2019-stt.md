---
id: "yu-2019-stt"
title: "Speculative Taint Tracking (STT): A Comprehensive Protection for Speculatively Accessed Data"
authors: ["Jiyong Yu", "Mengjia Yan", "Artem Khyzha", "Adam Morrison", "Josep Torrellas", "Christopher W. Fletcher"]
year: 2019
venue: "MICRO 2019, pp. 954-968"
doi: "10.1145/3352460.3358274"
source: "https://doi.org/10.1145/3352460.3358274"
status: "catalogued"
topics: ["microarchitectural-security", "computer-architecture"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Speculative taint tracking (STT)

[Publication DOI](https://doi.org/10.1145/3352460.3358274) · [Direction catalogue](index.md)

## Reading focus

STT lets speculation continue while delaying instructions that could transmit sensitive data. Its performance argument depends on how often that restriction lands on the critical path.

- Defines the access/transmit distinction that later secure-speculation work reuses.

Reading tier: core for secure microarchitecture.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: speculative execution attacks can read and leak program data, so the paper proposes a defense that delays instructions consuming speculatively accessed data until they are no longer speculative.

## Questions for the full paper

- How are transmitters defined, and which channels (cache, port contention, implicit channels) are covered?
- What overhead is reported, and on which simulated core?
- How hard would STT be to add to an RTL core such as BOOM?

## Connections

[Spectre](kocher-2019-spectre.md) · [SonicBOOM](../../computer-architecture/papers/zhao-2020-sonicboom.md) · [Unique program execution checking (UPEC)](fadiheh-2019-upec.md)
