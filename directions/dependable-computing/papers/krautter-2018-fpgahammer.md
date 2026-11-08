---
id: "krautter-2018-fpgahammer"
title: "FPGAhammer: Remote Voltage Fault Attacks on Shared FPGAs, suitable for DFA on AES"
authors: ["Jonas Krautter", "Dennis R. E. Gnad", "Mehdi B. Tahoori"]
year: 2018
venue: "IACR Transactions on Cryptographic Hardware and Embedded Systems 2018(3), 44–68"
doi: "10.13154/tches.v2018.i3.44-68"
source: "https://doi.org/10.13154/tches.v2018.i3.44-68"
status: "prior-work-imported"
topics: ["hardware-security", "fpgas", "fault-injection", "side-channels"]
added: "2026-11-03"
source_checked: "2026-11-03"
read_version: null
---

# FPGAhammer

[Published article](https://doi.org/10.13154/tches.v2018.i3.44-68) · Uploaded sources: `FPGAHammer.pdf` and `ojsadmin,+TCHES2018_3_03.pdf` (identical PDF files)

## Mechanism and evidence

Two FPGA tenants can occupy separate regions and still draw power from the same network. Krautter, Gnad and Tahoori ask whether load in one region can change timing in the other. The paper distinguishes coarse system outages from faults that change an individual computation's output. In a laboratory proof of concept, the authors observe timing faults affecting an AES design and report that those outputs can support differential fault analysis (DFA). The evaluation spans multiple FPGA boards and considers differences between nominally similar devices, linking susceptibility to platform and timing characteristics. Its contribution is an experimentally supported warning that logical partitioning does not by itself eliminate electrical interactions between FPGA regions. The paper does not demonstrate a compromise of a production multi-tenant cloud deployment, and its results should not be generalized to all AES implementations or FPGA families.

## Details to check

- Map the assumed adversary/victim isolation boundary, shared physical resources and application interface; distinguish a conceptual remote deployment from the test platforms actually used (Section 2).
- Trace the scientific reasoning from PDN variation to timing-margin erosion and incorrect outputs, without treating the demonstrator as a universal fault model (Sections 2–4).
- Separate the three evaluation layers: electrical/logic fault observations, correctness of the AES computation and the paper's proof-of-concept cryptanalytic consequence (Sections 3–4).
- Audit which experimental differences are attributable to board/platform configuration, manufacturing variation and timing constraints; do not average unlike cases into a universal fault rate (Section 4).
- Identify what static timing analysis can and cannot establish when runtime supply conditions depart from design assumptions (Sections 4–5).
- Review the authors' defensive discussion at the level of electrical safeguards, timing resilience, runtime monitoring and isolation policy, noting which ideas are suggestions rather than tested protections (Section 5).

## Comparison

[Gnad et al. (2017)](gnad-2017-voltage-drop-fpga.md) focus on denial of service from severe electrical disturbances; FPGAhammer studies the distinct integrity and confidentiality consequences of computational faults. [An Inside Job](schellenberg-2018-inside-job.md) examines passive observation through the same broad PDN-sharing issue rather than fault injection. [PWNN](xu-2026-pwnn.md) presents a different workload setting and newer devices. A successful laboratory DFA demonstration is not a measured cloud-wide risk rate or a validation of another paper's detection claims.

Reading state: Both uploaded FPGAhammer PDFs were checked and found byte-identical. One source-grounded note is retained; no attack reproduction or independent validation is claimed.
