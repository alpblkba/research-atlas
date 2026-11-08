---
id: "gnad-2017-voltage-drop-fpga"
title: "Voltage Drop-based Fault Attacks on FPGAs using Valid Bitstreams"
authors: ["Dennis R. E. Gnad", "Fabian Oboril", "Mehdi B. Tahoori"]
year: 2017
venue: "27th International Conference on Field Programmable Logic and Applications (FPL), 1–7"
doi: "10.23919/FPL.2017.8056840"
source: "https://doi.org/10.23919/FPL.2017.8056840"
status: "prior-work-imported"
topics: ["hardware-security", "fpgas", "fault-injection", "reliability"]
added: "2026-11-03"
source_checked: "2026-11-03"
read_version: null
---

# Voltage Drop-based Fault Attacks on FPGAs using Valid Bitstreams

[Published article](https://doi.org/10.23919/FPL.2017.8056840) · Uploaded source: `Voltage_drop-based_fault_attacks_on_FPGAs_using_valid_bitstreams.pdf`

## Mechanism and evidence

Gnad, Oboril and Tahoori look at components that the FPGA separates logically but powers from the same network. User-configurable logic can therefore affect availability elsewhere on the device. Their experiments show that configurations accepted as valid by the ordinary FPGA design flow can nevertheless generate electrical disturbances severe enough to stop the tested devices or attached systems. Some observed failures required manual power cycling to restore service. The authors study multiple FPGA generations and an FPGA-based SoC, framing the weakness as a gap between logical design isolation and electrical isolation. The work concerns denial of service and platform reliability; it does not demonstrate cryptographic key recovery or a fault attack against a particular encryption round. The reported outcomes are measurements on the authors' test hardware, not evidence that all deployed cloud FPGA platforms exhibit the same failure behavior.

## Details to check

- Reconstruct the authors' threat model: what configuration authority is granted to an untrusted user, which components share the PDN, and what availability guarantee the system is expected to provide (Introduction and Section II).
- Separate the physical explanation of supply-voltage variation, circuit delay and system malfunction from claims about a specific attacker's capabilities (Sections II and III).
- Inspect how the paper distinguishes ordinary vendor-valid configuration from the stronger claim that a configuration is electrically safe under all operating conditions (Sections I and III).
- Record the tested FPGA families, SoC setting, observed recovery behavior and variation between experiments without extending the outcome to untested architectures (Section IV).
- Examine the observability and mitigation discussion: electrical monitoring, conservative operating limits, isolation and practical constraints on detecting short-lived disturbances (Section IV).
- Note that a crash requiring power cycling is a persistent loss of availability until intervention, not necessarily permanent physical destruction of the device.

## Comparison

[FPGAhammer](krautter-2018-fpgahammer.md) extends the shared-PDN fault argument from severe availability failures to timing faults affecting a cryptographic computation. [PWNN](xu-2026-pwnn.md) later considers input-dependent accelerator activity in related shared-power threat models. These studies differ in goal, experimental platforms and observables. The FPL paper does not itself establish the later papers' claims about differential fault analysis, and successful logical/bitstream checks should not be interpreted as complete validation of electrical robustness.

Reading state: Uploaded PDF inspected for the threat model, experimental scope, availability claims and mitigation discussion; this is an initial source-grounded reading note, not a reproduction or a generalized vulnerability assessment.
