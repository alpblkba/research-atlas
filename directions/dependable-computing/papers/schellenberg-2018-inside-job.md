---
id: "schellenberg-2018-inside-job"
title: "An Inside Job: Remote Power Analysis Attacks on FPGAs"
authors: ["Falk Schellenberg", "Dennis R. E. Gnad", "Amir Moradi", "Mehdi B. Tahoori"]
year: 2018
venue: "Design, Automation & Test in Europe Conference & Exhibition (DATE), 1111–1116"
doi: "10.23919/DATE.2018.8342177"
source: "https://doi.org/10.23919/DATE.2018.8342177"
status: "prior-work-imported"
topics: ["hardware-security", "fpgas", "side-channels"]
added: "2026-11-03"
source_checked: "2026-11-03"
read_version: null
---

# An Inside Job

[Published conference paper](https://doi.org/10.23919/DATE.2018.8342177) · Uploaded source: `2018-012.pdf`

## Mechanism and evidence

Schellenberg et al. study what one FPGA tenant can learn about another by observing the shared power network while the victim continues to compute. The authors present a proof of concept in which FPGA-internal delay sensors observe activity-dependent voltage changes from a logically separate cryptographic core. Their evaluation uses a Spartan-6 device on a SAKURA-G board, with AES as the case study, and compares internal observations with an external power-measurement reference. The paper reports a practical side-channel demonstration under its laboratory conditions. The architectural lesson is that an absence of explicit signal connections between two modules does not imply an absence of measurable physical coupling. The experiments do not measure confidentiality loss in a live commercial cloud, and the paper's sensor results depend on the tested platform and measurement setting.

## Details to check

- Describe the two high-level shared-resource scenarios in the threat model and identify the trust boundary not covered by logical netlist separation (Section II).
- Understand why a circuit's data-dependent power activity can become observable as a variation in a shared electrical resource, while keeping separate the physical measurement from the inference made from it (Sections II–III).
- Examine the validation methodology and compare the internal sensor observations against external reference measurements; identify where instrumentation and laboratory access differ from the proposed remote-use scenario (Sections III–IV).
- Record the board, target core, experimental environment and spatial-separation assumptions; avoid extrapolating performance to newer FPGA families or unrelated workloads (Sections III–IV).
- Distinguish evidence of a statistically useful signal from broad claims of reliable leakage under all possible conditions, placements and noise sources (Section IV).
- Consider defensive implications for partitioning, third-party IP review, physical side-channel isolation and runtime observability; note that the paper is primarily a vulnerability demonstration rather than a measured defense evaluation.

## Comparison

[FPGAhammer](krautter-2018-fpgahammer.md) and [PWNN](xu-2026-pwnn.md) focus on active disturbances and loss of computational integrity, whereas this DATE paper studies a side channel that reveals information through passive observation. The three share a PDN-isolation theme but should not be described as the same attack or compared using a common success-rate metric. The protection goals of [Meschkov et al. (2025)](meschkov-2025-physically-secure-fpga.md) also require separate treatment: secure logic styles and FPGA-wide electrical isolation are distinct architectural questions.

Reading state: Uploaded DATE paper inspected for threat assumptions, internal-versus-external measurement framing and experimental scope; this note does not establish results on untested devices or reproduce the side-channel experiment.
