---
id: "zick-2013-sensing-voltage-transients"
title: "Sensing Nanosecond-Scale Voltage Attacks and Natural Transients in FPGAs"
authors: ["Kenneth M. Zick", "Meeta Srivastav", "Wei Zhang", "Matthew French"]
year: 2013
venue: "FPGA 2013, pp. 101-104"
doi: "10.1145/2435264.2435283"
source: "https://doi.org/10.1145/2435264.2435283"
status: "catalogued"
topics: ["physical-security"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Sensing nanosecond-scale voltage attacks in FPGAs

[Publication DOI](https://doi.org/10.1145/2435264.2435283) · [Direction catalogue](index.md)

## Reading focus

Zick et al. use FPGA logic to sense fast voltage transients. My task5 carry-chain TDC belongs to that family, so the calibration and time resolution are the parts to compare.

- Shows that fabric activity can push the supply outside specification, the precondition for the droop faults later shown in FPGAhammer.

Reading tier: core for the sensor thread.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: heavy activity in FPGA fabric can cause voltage overshoot and undershoot beyond specification; an existing on-chip voltage sensor proved inadequate, and the authors propose a sensor built from reconfigurable logic that samples much faster than the Xilinx ADC.

## Questions for the full paper

- How is the sensor calibrated, and which resolution and sample rate are reported?
- How does it compare with the 64-tap carry-chain TDC used in task5?
- Can it separate attack-induced droop from natural transients, which the task5 alarm detected but could not attribute per ciphertext?

## Connections

[Power distribution attacks in multi-user FPGAs](provelengios-2019-power-distribution-attacks.md) · [Active fences](krautter-2019-active-fences.md) · [Voltage Drop-based Fault Attacks on FPGAs using Valid Bitstreams](../../dependable-computing/papers/gnad-2017-voltage-drop-fpga.md)
