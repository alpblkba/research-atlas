---
id: "xu-2026-pwnn"
title: "PWNN: Power-Wasting Neural Network As Remote Fault Injector"
authors: ["Huashuangyang Xu", "Sergej Meschkov", "Vincent Meyers", "Mehdi Tahoori"]
year: 2026
venue: "IACR Transactions on Cryptographic Hardware and Embedded Systems 2026(1), 448–471"
doi: "10.46586/tches.v2026.i1.448-471"
source: "https://doi.org/10.46586/tches.v2026.i1.448-471"
status: "prior-work-imported"
topics: ["hardware-security", "fpgas", "fault-injection"]
added: "2026-11-03"
source_checked: "2026-11-03"
read_version: null
---

# PWNN

[Published article](https://doi.org/10.46586/tches.v2026.i1.448-471) · Uploaded source: `TCHES2026_1_18.pdf`

## Mechanism and evidence

Xu et al. examine what happens when FPGA regions that appear isolated in the design still share a physical power network. They introduce PWNN, a binarized-neural-network-based example of workload-dependent power activity whose behavior is not adequately characterized by static structural design-rule checks. The paper uses an open-source neural-network-to-FPGA tool flow and reports experimental timing-fault effects on two AMD platforms, PYNQ-Z2 and ZCU104, in co-located cryptographic and arithmetic test designs. Its evaluation includes a Differential Fault Analysis (DFA) demonstration involving an AES-128 core. The architectural lesson is that ordinary-looking accelerator structure and successful pre-deployment checks do not establish safe runtime electrical behavior, especially when independent logic regions share a power-delivery network. The real-board demonstrations support a shared-resource security concern; they do not constitute a reported attack against a production multi-tenant cloud service.

## Details to check

- Define the paper's precise isolation and access assumptions: separate logical regions, shared power delivery, co-located circuits and the difference between the authors' laboratory platforms and a deployed multi-tenant cloud environment (Section 2.1).
- Separate the general hardware mechanism, input-dependent switching and power-delivery transients, from the application-layer claim about neural-network accelerators and from the cryptanalytic demonstration (Sections 2 and 3).
- Identify what vendor structural checks and static analysis are intended to guarantee, which runtime properties they do not assess, and the defensive significance of that coverage gap (Sections 2.2 and 5).
- Record the evaluated FPGA families, victim classes and experimental observables; distinguish timing/fault occurrence, output integrity and the higher-level implications for confidentiality (Section 4).
- Critically assess external validity: platform dependence, shared-power assumptions, limits of generalizing laboratory experiments to cloud operator policies, and the distinction between observed behavior and the authors' broader security claims (Sections 4 and 5).
- Examine the proposed defensive directions, particularly runtime monitoring, fault/error detection and operational isolation, without treating any one mitigation as experimentally established in this paper (Sections 5 and 6).

## Comparison

[Meschkov et al. (2025)](meschkov-2025-physically-secure-fpga.md) develop a secure reconfigurable fabric and investigate masking, dual-rail logic and fault detection. PWNN instead studies a runtime threat arising from a shared physical resource on conventional FPGA platforms. The studies are complementary but do not supply a head-to-head evaluation of one another's defenses. Nor should the paper's use of a neural-network implementation be generalized into a claim that ordinary AI accelerators are malicious; the threat depends on adversarial use and the stated hardware/isolation conditions.

Reading state: Uploaded PDF inspected for the threat model, architecture-level argument, evaluation scope and limitations; no reproduction or independent validation of cloud-scale exploitability is claimed.
