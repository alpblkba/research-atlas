# Papers: Physical security

These are the sources I can return to for this direction. Each note records how far the source check went.

- [Secure FPGA and toolchain](meschkov-2025-secure-fpga-toolchain.md)
- [PWNN](xu-2026-pwnn.md)
- [Automated FPGA masking](mueller-2023-automated-masking-fpga.md)
- [Secure reconfigurable system dissertation](meschkov-2026-secure-reconfigurable-system.md)

## Foundations and multi-tenant FPGA literature, added 2026-11-06

Several of these are already cited in the alpblkba.dev notes on CPA, DFA, voltage droop and the SRAM PUF; the notes say which.

### Power and fault analysis

| Paper | Venue | Role |
|---|---|---|
| [Differential power analysis](kocher-1999-dpa.md) | CRYPTO 1999 | origin of differential power analysis |
| [Correlation power analysis](brier-2004-cpa.md) | CHES 2004 | method used in the task3 CPA |
| [Differential fault analysis of secret key cryptosystems](biham-1997-dfa.md) | CRYPTO 1997 | origin of differential fault analysis |
| [Piret-Quisquater DFA on AES](piret-2003-dfa-spn-aes.md) | CHES 2003 | key recovery targeted by the task4 DFA |
| [FPGA intrinsic PUFs](guajardo-2007-fpga-intrinsic-pufs.md) | CHES 2007 | SRAM power-up PUFs on FPGAs |

### On-chip sensing and multi-tenant FPGAs

| Paper | Venue | Role |
|---|---|---|
| [Sensing nanosecond-scale voltage attacks in FPGAs](zick-2013-sensing-voltage-transients.md) | FPGA 2013 | early fast on-chip voltage sensor |
| [Power distribution attacks in multi-user FPGAs](provelengios-2019-power-distribution-attacks.md) | FPL 2019 | cross-tenant supply disturbance |
| [Active fences](krautter-2019-active-fences.md) | ICCAD 2019 | ring-oscillator noise as a defense |

### Software-triggered faults

| Paper | Venue | Role |
|---|---|---|
| [CLKSCREW](tang-2017-clkscrew.md) | USENIX Security 2017 | software-driven DVFS faults on Arm |
| [Plundervolt](murdock-2020-plundervolt.md) | IEEE S&P 2020 | software-driven undervolting faults on SGX |

[Direction overview](../index.md)
