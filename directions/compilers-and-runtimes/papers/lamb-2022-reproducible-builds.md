---
id: "lamb-2022-reproducible-builds"
title: "Reproducible Builds: Increasing the Integrity of Software Supply Chains"
authors: ["Chris Lamb", "Stefano Zacchiroli"]
year: 2022
venue: "IEEE Software 39(2), pp. 62-70"
doi: "10.1109/MS.2021.3073045"
source: "https://doi.org/10.1109/MS.2021.3073045"
status: "catalogued"
topics: ["compilers-and-runtimes", "systems-reliability"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Reproducible builds

[Publication DOI](https://doi.org/10.1109/MS.2021.3073045) · [Direction catalogue](index.md)

## Reading focus

If two people build the same source independently, do they get the same bytes? That gives me a concrete check on the toolchain after Thompson's compiler example.

- Relevant to open-source supply chain work and to any research artifact released with a paper.

Reading tier: background.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: reviewing open-source code does not make the built executables trustworthy, and the article examines reproducible builds as a way to verify that binaries match their source. OpenAlex lists 2021 as the publication year (online first); the issue is IEEE Software 39(2).

## Questions for the full paper

- Which sources of nondeterminism are most common (timestamps, paths, ordering)?
- How far had distributions such as Debian progressed according to the article?
- How does Nix's store model compare?

## Connections

[Reflections on trusting trust](thompson-1984-trusting-trust.md) · [Nix](dolstra-2004-nix.md)
