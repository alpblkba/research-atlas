---
id: "zhang-2026-apple-interrupt-side-channels"
title: "Towards Practical Interrupt Side-Channel Attacks on macOS for Apple Silicon"
authors: ["Xin Zhang", "Chang Liu", "Jiajun Zou", "Yi Yang", "Qingni Shen", "Zhi Zhang", "Trevor E. Carlson"]
year: 2026
venue: "ISCA 2026"
doi: null
source: "https://www.comp.nus.edu.sg/~tcarlson/pdfs/zhang2026tpisaomfas.pdf"
status: "catalogued"
topics: ["microarchitectural-security", "operating-systems"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Interrupt side channels on Apple Silicon

[Source](https://www.comp.nus.edu.sg/~tcarlson/pdfs/zhang2026tpisaomfas.pdf) · [ISCA 2026 program](https://www.iscaconf.org/isca2026/program/) · [Direction catalogue](index.md)

## Reading focus

Interrupt delivery crosses the kernel and the SoC. On Apple Silicon the timing of that delivery can expose activity across a boundary, so both the hardware path and OS policy matter.

- Its detection technique relies on a macOS kernel behavior around the x18 register, a reminder that an OS mitigation can create new observable state.
- Reverse-engineers how Apple's interrupt controller routes shared peripheral interrupts, relevant to SoC-level interrupt routing and inter-processor communication.

Reading tier: optional, recent.

## Source record

Source check by agent, 2026-11-06: abstract from the author PDF; venue from the ISCA 2026 program.

Author PDF abstract: the authors propose TIDE, which detects interrupts through a macOS behavior around the user-visible x18 register under Apple's Double Map mitigation, find that Apple's interrupt controller spreads shared peripheral interrupts across all active cores, and report website fingerprinting accuracy of 93.8% closed-world and 91.2% open-world, a timer-less covert channel at 111.65 b/s and key extraction from Cloudflare CIRCL v1.1. The venue comes from the ISCA 2026 program; the PDF does not print it. No award is marked for this paper on the program page.

## Questions for the full paper

- Which macOS versions expose the x18 behavior, and has Apple changed it since?
- How was the interrupt distribution policy reverse-engineered?
- How does the attacker model compare with the SysBumps and loop-counting attacks it improves?

## Connections

[PACMAN](ravichandran-2022-pacman.md) · [GoFetch](chen-2024-gofetch.md) · [Helium](archer-2026-helium.md)
