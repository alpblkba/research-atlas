---
id: "chen-2025-stratus"
title: "STRATUS: A Multi-agent System for Autonomous Reliability Engineering of Modern Clouds"
authors: ["Yinfang Chen", "Jiaqi Pan", "Jackson Clark", "Yiming Su", "Noah Zheutlin", "Bhavya Bhavya", "Rohan Arora", "Yu Deng", "Saurabh Jha", "Tianyin Xu"]
year: 2025
venue: "arXiv preprint; revised 2026"
doi: "10.48550/arXiv.2506.02009"
source: "https://arxiv.org/abs/2506.02009"
status: "catalogued"
topics: ["systems-reliability", "dependable-computing"]
added: "2026-11-03"
source_checked: "2026-11-03"
read_version: null
---
# STRATUS

[Source: arXiv v2](https://arxiv.org/abs/2506.02009v2) · [Systems reliability direction](../index.md)

## Evidence from the abstract

STRATUS splits cloud incident response into roles such as diagnosis and mitigation and coordinates its LLM agents with a state machine. The paper introduces Transactional No-Regression (TNR) as a safety specification for exploring and applying mitigations. It evaluates across AIOpsLab and ITBench; any success-rate claims apply to those test conditions and should not be read as production reliability guarantees.

## Questions to bring to the full paper

- Define TNR precisely: what state is snapshotted, what changes are reversible, and how is regression detected?
- Distinguish detecting a fault, selecting a mitigation and proving a service has recovered.
- Which oracle or observed metrics are available to the agent itself, and which are used only by the evaluator?
- Compare the system's safety guarantees to the failure coverage and noise model offered by [SREGym](clark-2026-sregym.md).

The cited SREGym evaluation document lists this as a recommended/context source, not as a personalized endorsement invented by the atlas. Provenance.

Reading state: Catalogued; abstract checked, formal definition and evaluation tables pending.
