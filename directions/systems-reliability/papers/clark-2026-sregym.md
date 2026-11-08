---
id: "clark-2026-sregym"
title: "SREGym: A Live Benchmark for AI SRE Agents with High-Fidelity Failure Scenarios"
authors: ["Jackson Clark", "Yiming Su", "Saad Mohammad Rafid Pial", "Yifang Tian", "Lily Gniedziejko", "Hans-Arno Jacobsen", "Yinfang Chen", "Tianyin Xu"]
year: 2026
venue: "arXiv preprint"
doi: "10.48550/arXiv.2605.07161"
source: "https://arxiv.org/abs/2605.07161"
status: "catalogued"
topics: ["systems-reliability", "dependable-computing"]
added: "2026-11-03"
source_checked: "2026-11-03"
read_version: null
---
# SREGym

[Recommended v2 source](https://arxiv.org/abs/2605.07161v2) · [arXiv record](https://arxiv.org/abs/2605.07161) · [Systems reliability direction](../index.md)

## Evidence from the abstract

SREGym injects faults and background noise into running cloud-native stacks to evaluate SRE agents. Its design emphasizes low-level, concurrent and correlated failures rather than only clean single-fault incidents. The authors' abstract reports a suite of 90 problems. This is a benchmark contribution; the benchmark's claimed fidelity must be assessed separately from any agent's measured success.

## The questions worth reading for

- What is the incident ground truth, and is it kept separate from the information visible to the agent?
- Which faults/noise are realistic abstractions and which depend on an implementation-specific harness?
- What constitutes a successful mitigation, and can a post-recovery regression escape the grading oracle?
- How are retries, time budgets and irreversible changes counted in an agent score?

## Recommendation provenance

The SREGym evaluation document shared in Tianyin Xu's context lists arXiv:2605.07161v2; the public arXiv record may show a newer version. Track the version actually read before quoting numbers. Source log. Compare with [STRATUS](chen-2025-stratus.md), an agent rather than a benchmark.

Reading state: Catalogued, source abstract checked, detailed reading pending.
