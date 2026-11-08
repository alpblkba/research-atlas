---
id: "kim-2014-flipping-bits"
title: "Flipping Bits in Memory Without Accessing Them: An Experimental Study of DRAM Disturbance Errors"
authors: ["Yoongu Kim", "Ross Daly", "Jeremie Kim", "Chris Fallin", "Ji Hye Lee", "Donghyuk Lee", "Chris Wilkerson", "Konrad Lai", "Onur Mutlu"]
year: 2014
venue: "ISCA 2014"
doi: "10.1109/ISCA.2014.6853210"
source: "https://users.ece.cmu.edu/~yoonguk/papers/kim-isca14.pdf"
status: "catalogued"
topics: ["memory-systems", "dependable-computing"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Flipping bits in memory without accessing them

[Publication DOI](https://doi.org/10.1109/ISCA.2014.6853210) · [Source](https://users.ece.cmu.edu/~yoonguk/papers/kim-isca14.pdf) · [Author PDF](https://users.ece.cmu.edu/~yoonguk/papers/kim-isca14.pdf) · [Direction catalogue](index.md)

## Reading focus

TRRespass assumes the reader already knows what repeated DRAM activations can disturb. Kim et al. characterize that effect and propose PARA, which gives the later mitigation papers an early comparison point.

- It is a DRAM characterization study before it is a security paper, which is why its canonical note lives in memory systems and is linked from dependable computing.
- Provides the DDR3-era baseline facts that the CDNC seminar papers update for DDR4, DDR5 with PRAC, and GDDR6.

Reading tier: background citation for the seminar, core for memory systems.

## Source record

Source check by agent, 2026-11-06: metadata from Crossref; abstract from the author PDF.

The author PDF abstract was checked. The authors report disturbance errors in 110 of 129 tested DDR3 modules from three manufacturers, trigger bit flips from a user-level program on Intel Sandy Bridge, Ivy Bridge and Haswell and on AMD Piledriver systems with as few as 139K accesses, attribute the errors to repeated wordline toggling, and propose PARA, a probabilistic adjacent-row refresh. These are 2014 DDR3 results and do not describe DDR4 or DDR5 thresholds.

## Questions for the full paper

- How was the test infrastructure built (FPGA-based tester versus real systems), and what does each part measure?
- How is PARA's probability chosen, and what security argument does the paper give for it?
- Which observations were revised by later characterization of DDR4 and DDR5 devices?

## Connections

[TRRespass](../../dependable-computing/papers/frigo-2020-trrespass.md) · [QPRAC](../../dependable-computing/papers/woo-2025-qprac.md) · [Ramulator 2.0](luo-2024-ramulator2.md) · [DRAMSys4.0](steiner-2022-dramsys4.md) · [Rowhammer mitigation map](../rowhammer-mitigations.md)
