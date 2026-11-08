---
id: "xu-2026-pwnn"
title: "PWNN: Power-Wasting Neural Network As Remote Fault Injector"
authors: ["Huashuangyang Xu", "Sergej Meschkov", "Vincent Meyers", "Mehdi Tahoori"]
year: 2026
venue: "IACR TCHES 2026(1), 448–471"
doi: "10.46586/tches.v2026.i1.448-471"
source: "https://doi.org/10.46586/tches.v2026.i1.448-471"
status: "catalogued"
topics: ["physical-security", "dependable-computing"]
added: "2026-11-03"
source_checked: "2026-11-03"
read_version: null
---
# PWNN: Power-Wasting Neural Network As Remote Fault Injector

[Source: TCHES 2026](https://doi.org/10.46586/tches.v2026.i1.448-471) · [KITopen record](https://publikationen.bibliothek.kit.edu/1000190457) · [Physical security direction](../index.md)

## Evidence from the abstract

Xu, Meschkov, Meyers and Tahoori ask whether a neural-network workload can cause a timing fault in another tenant's circuit through the shared FPGA power supply. Their evaluation includes AMD ZCU104 and PYNQ-Z2 boards and a co-located AES-128 target; the authors report that conventional pre-implementation checks do not fully characterize this runtime threat. This is a high-level summary of the published abstract, not a reproduction or instruction for inducing faults.

## Questions for the CDNC seminar

- Which isolation boundary, voltage/power assumption and adversary capability does the paper depend on?
- What is the difference between functional correctness of a design and physical safety of co-located execution?
- Which evidence distinguishes correlation, measured faults and the paper's security conclusion?
- How does this setting differ from the secure FPGA *fabric/mapping* approach in [Meschkov et al. 2025](meschkov-2025-secure-fpga-toolchain.md)?

I know the PYNQ-Z2 from my FPGA work. The paper does not establish the same behavior in my earlier board design; that comparison would need matching workload, placement and power conditions.

Reading state: Catalogued, abstract checked. No experiment planned.
