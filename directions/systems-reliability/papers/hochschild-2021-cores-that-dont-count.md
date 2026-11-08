---
id: "hochschild-2021-cores-that-dont-count"
title: "Cores that don't count"
authors: ["Peter H. Hochschild", "Paul Turner", "Jeffrey C. Mogul", "Rama Govindaraju", "Parthasarathy Ranganathan", "David E. Culler", "Amin Vahdat"]
year: 2021
venue: "HotOS 2021, pp. 9-16"
doi: "10.1145/3458336.3465297"
source: "https://doi.org/10.1145/3458336.3465297"
status: "catalogued"
topics: ["systems-reliability", "dependable-computing"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Cores that don't count

[Publication DOI](https://doi.org/10.1145/3458336.3465297) · [Direction catalogue](index.md)

## Reading focus

Google reports cores that pass manufacturing tests and later return incorrect results in production. A service incident can therefore start below the layers its normal health checks observe.

- Bridges hardware reliability (defects, aging, voltage margins) and fleet operations.

Reading tier: core, short.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: processors assumed to fail cleanly can have subtle defects that pass manufacturing tests and silently produce wrong results, which is hard to work around in software.

## Questions for the full paper

- How are such cores detected in the fleet, and how often?
- Which instructions or units are implicated?
- How do the authors divide responsibility between hardware and software?

## Connections

[Silent data corruptions at scale](dixit-2021-sdc-at-scale.md) · [Cerberus](../../memory-systems/papers/kim-2026-cerberus.md) · [Gray failure](huang-2017-gray-failure.md)
