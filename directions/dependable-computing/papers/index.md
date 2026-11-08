# Papers: dependable computing

These are the sources I can return to for this direction. Each note records how far the source check went. The 4 November 2026 seminar set contains 19 named papers under RowHammer Across Modern Memory Architectures: Attacks, Defenses, and AI Security.

## Core seminar literature

Five selected papers; four deep reads and one focused/short read (QPRAC).

| Paper | Venue | Why chosen / role |
|---|---|---|
| [When Mitigations Backfire](woo-2025-when-mitigations-backfire.md) | ISCA 2025 | the central case of a protection mechanism introducing a different security exposure |
| [QPRAC](woo-2025-qprac.md) | HPCA 2025 | establish PRAC, ABO, RFM and mitigation-queue concepts needed for WMB |
| [Chronus](canpolat-2025-chronus.md) | HPCA 2025 | connect RowHammer thresholds to PRAC security and scaling cost |
| [GPUHammer](lin-2025-gpuhammer.md) | USENIX Security 2025 | compare GPU GDDR6 organization, access behavior and refresh constraints with CPU DRAM |
| [PRowhammer](shukla-2026-prowhammer.md) | ISCA 2026 | expose the dependency of GPU execution on host DRAM and shared libraries |

## Citation-only supporting literature

These 12 papers supply background or bounded comparisons. They do not enlarge the five-paper core.

| Paper | Venue | Why chosen / role |
|---|---|---|
| [TRRespass](frigo-2020-trrespass.md) | IEEE S&P 2020 | explain why TRR did not settle the RowHammer problem |
| [Blacksmith](jattke-2022-blacksmith.md) | IEEE S&P 2022 | follow TRRespass with the role of non-uniform access patterns |
| [ColumnDisturb](yuksel-2025-columndisturb.md) | MICRO 2025 | question the locality assumptions used to choose which victims need refresh |
| [ColumnKeeper](kakolyris-2026-columnkeeper.md) | ISCA 2026 | show an architectural response to the assumption challenged by ColumnDisturb |
| [LeakyHammer](bostanci-2025-leakyhammer.md) | MICRO 2025 | compare mitigation-induced timing leakage with WMB |
| [AutoPRAC](qu-2026-autoprac.md) | DRAMSec 2026 workshop | illustrate automated scrutiny of counting/reset policies |
| [Sigries / From Lab to Fleet](saroiu-2026-from-lab-to-fleet.md) | ISCA 2026 industry track | represent production constraints in a seminar otherwise dominated by research designs |
| [FiRM / From Fleet to Lab](taneja-2026-from-fleet-to-lab.md) | arXiv preprint | follow the deployed-design description with a critique of transition guarantees |
| [GPUThor](lin-2026-gputhor.md) | ACM CCS 2026 (accepted; forthcoming on 2026-11-04) | qualify ECC as a system-specific protection with a finite correction capability |
| [PrisonBreak](coalson-2024-prisonbreak.md) | arXiv preprint (v3 revised 2025) | distinguish alignment integrity from classification accuracy and code integrity |
| [PRAC on real hardware](kim-2025-prac-real-hardware.md) | IEEE Computer Architecture Letters 2025 | anchor the timing-cost discussion in measurements on real machines |
| [CnC-PRAC](lin-2025-cnc-prac.md) | DRAMSec 2025 workshop | show that PRAC overhead depends on counter-storage and update design choices |

## Optional research pool

Catalogued for navigation, with no obligation to cite, read deeply or reproduce.

| Paper | Venue | Possible role |
|---|---|---|
| [GPUBreach](lin-2026-gpubreach.md) | IEEE S&P 2026 | use only if the survey needs a contrast between model corruption and memory-isolation failure |
| [JENGA](abgrall-2026-jenga.md) | IEEE RTSS 2026 (accepted; forthcoming on 2026-11-04) | distinguish worst-case predictability from the average-performance metrics in PRAC studies |

## Other existing direction papers

These entries are retained from the earlier catalogue and are not added to the current seminar selection.

- [Voltage Drop-based Fault Attacks on FPGAs using Valid Bitstreams](gnad-2017-voltage-drop-fpga.md)
- [FPGAhammer](krautter-2018-fpgahammer.md)
- [Design and Implementation of a Physically Secure Open-Source FPGA and Toolchain](meschkov-2025-physically-secure-fpga.md)
- [Side-Channel Attack with Fault Analysis on Memristor-based Computation-in-Memory](sapui-2024-memristor-cim-sidechannel.md)
- [An Inside Job: Remote Power Analysis Attacks on FPGAs](schellenberg-2018-inside-job.md)
- [PWNN: Power-Wasting Neural Network As Remote Fault Injector](xu-2026-pwnn.md)

[Seminar core index](../seminar/papers/index.md) · [Seminar overview](../seminar/README.md) · [Direction overview](../index.md)
