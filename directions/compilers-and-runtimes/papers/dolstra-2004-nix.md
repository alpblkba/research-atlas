---
id: "dolstra-2004-nix"
title: "Nix: A Safe and Policy-Free System for Software Deployment"
authors: ["Eelco Dolstra", "Merijn de Jonge", "Eelco Visser"]
year: 2004
venue: "LISA 2004"
doi: null
source: "https://static.usenix.org/event/lisa04/tech/dolstra.html"
status: "catalogued"
topics: ["compilers-and-runtimes", "systems-reliability"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Nix

[Source](https://static.usenix.org/event/lisa04/tech/dolstra.html) · [USENIX PDF](https://static.usenix.org/event/lisa04/tech/full_papers/dolstra/dolstra.pdf) · [Direction catalogue](index.md)

## Reading focus

Nix gives builds distinct store paths derived from their inputs, so different versions can coexist. I want to trace which inputs determine the path before drawing conclusions about reproducibility.

- Links build reproducibility, supply chain integrity and research-artifact packaging.

Reading tier: optional.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the USENIX LISA 2004 abstract page.

USENIX abstract: deployment tools are unreliable and inflexible, so Nix gives each component instance a unique path derived from a cryptographic hash, allowing multiple versions side by side and safe upgrades.

## Questions for the full paper

- What goes into the hash, and what does that guarantee about build inputs?
- Where does the 2004 design leak impurity (network, system time)?
- How does the store model interact with reproducible builds?

## Connections

[Reproducible builds](lamb-2022-reproducible-builds.md) · [Reflections on trusting trust](thompson-1984-trusting-trust.md)
