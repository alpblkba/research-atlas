---
id: "meschkov-2025-physically-secure-fpga"
title: "Design and Implementation of a Physically Secure Open-Source FPGA and Toolchain"
authors: ["Sergej Meschkov", "Daniel Lammers", "Mehdi B. Tahoori", "Amir Moradi"]
year: 2025
venue: "IACR Transactions on Cryptographic Hardware and Embedded Systems 2025(3), 542–582"
doi: "10.46586/tches.v2025.i3.542-582"
source: "https://doi.org/10.46586/tches.v2025.i3.542-582"
status: "prior-work-imported"
topics: ["hardware-security", "fpgas", "side-channels"]
added: "2026-11-03"
source_checked: "2026-11-03"
read_version: null
---

# Design and Implementation of a Physically Secure Open-Source FPGA and Toolchain

[Published article](https://doi.org/10.46586/tches.v2025.i3.542-582) · Uploaded source: `TCHES2025_3_20-1.pdf`

## Mechanism and evidence

Meschkov et al. design the FPGA fabric and the HDL-to-bitstream flow together so that physical protection is part of the mapping process. Their case study combines first-order Boolean masking with dual-rail pre-charge/hiding techniques, using modified LMDPL and WDDL-derived secure gadgets to address side-channel analysis (SCA) and provide detection of classes of fault-injection (FI) events. The design flow integrates open-source tools including AGEMA, FABulous, Yosys, nextpnr and BitMan. The paper provides gate-level design and simulation results, area estimates against secure implementations on a conventional FABulous-style fabric, and physical SCA measurements of a small secure fabric emulated on a commercial FPGA, rather than measurements from fabricated custom secure-fabric silicon. The reported roughly 85% area reduction concerns the paper's protected-design mapping comparison; it is not an 85% reduction compared with an unprotected design. In its first-order TVLA experiment, no leakage was detected over 100 million traces; this is a test result under the stated setup and model, not a general proof of absence of leakage.

## Details to check

- Reconstruct the threat model and the distinction between first-order masking, hiding, dual-rail encoding, glitch resistance and fault detection (Sections 2 and 3).
- Trace how secure gadgets are composed into reconfigurable tiles, how share domains and rail constraints are preserved, and where the automated HDL mapping and bitstream flow enforce those constraints (Sections 3 and 4).
- Separate the fabric's security assumptions from the assumptions of the formal probing model, logic-level fault simulations, and practical side-channel measurements; record which attack classes are outside the claims.
- Audit the baselines, gate-equivalent accounting and overhead exclusions in the area tables, especially the distinction between secure-on-conventional-fabric and secure-on-proposed-fabric mappings (Section 4.5).
- Examine the physical evaluation boundary: SAKURA-X/Kintex-7 emulation, size-limited AES S-Box test design, TVLA methodology, first-order findings and the paper's discussion of higher-order leakage (Sections 4.6 and 5.3).
- Review fault-detection limitations, configuration/bitstream security, test circuitry and other whole-device attack surfaces before treating gate-level guarantees as end-to-end device security (Sections 5.4–5.5).

## Comparison

[PWNN](xu-2026-pwnn.md) investigates input-dependent power-delivery interference between co-located FPGA designs. This paper studies a secure reconfigurable fabric, its mapping rules and its physical-security evaluation. They do not evaluate the same architecture, adversary access or security boundary, so PWNN's demonstrated platform-level fault behavior does not itself establish either a defeat or a validation of the secure-fabric proposal. In particular, first-order TVLA observations cannot be generalized to all side-channel orders, and modeled fault detection is not a guarantee against every physical disturbance.

Reading state: Uploaded PDF inspected for contributions, architecture, comparative area methodology, experimental setup and limitations; the note is an initial source-grounded reading record, not an independent security proof or reproduction.
