---
id: "lin-2025-gpuhammer"
title: "GPUHammer: Rowhammer Attacks on GPU Memories are Practical"
authors: ["Chris S. Lin", "Joyce Qu", "Gururaj Saileshwar"]
year: 2025
venue: "34th USENIX Security Symposium (USENIX Security '25), 5719–5738"
doi: null
source: "https://www.usenix.org/system/files/usenixsecurity25-lin-shaopeng.pdf"
status: "prior-work-imported"
topics: ["hardware-security", "memory-systems", "gpus", "rowhammer"]
added: "2026-11-03"
source_checked: "2026-11-04"
read_version: null
---

# GPUHammer

[USENIX publication](https://www.usenix.org/system/files/usenixsecurity25-lin-shaopeng.pdf) · Uploaded source: `SEC25_GPUHammer.pdf`

## Mechanism and evidence

Lin, Qu and Saileshwar test whether repeated accesses produce measurable disturbance faults in the GDDR memory of a discrete GPU. Their NVIDIA A6000/GDDR6 case study reports bit flips in multiple tested DRAM banks and evaluates the integrity consequences for deep-learning model parameters. The paper identifies GPU-specific architectural and memory-system differences from CPU Rowhammer work, including less visible memory mappings, distinct memory-access behavior and proprietary DRAM defenses. As a proof of impact, the study reports substantial prediction-accuracy degradation when model parameters are corrupted. The reported experiments establish a vulnerability on the evaluated GPU and memory setting, not a claim that all GPUs, all GDDR generations or all production multi-tenant deployments are susceptible. The authors discuss error-correction and other system-level resilience approaches, as well as the need to examine ML-model sensitivity to corruption.

## Details to check

- Identify the exact GPU, DRAM technology, firmware/system assumptions and scope of the experimental evidence; distinguish GDDR6 findings from HBM or other GPU generations (Sections 2 and evaluation).
- Track which measurements characterize DRAM address organization, fault occurrence and platform variability, and separate inference about underlying memory mechanisms from directly observed behavior.
- Separate a physical bit flip from the application-level consequence: weight representation, model sensitivity, output integrity and accuracy measured on particular workloads (evaluation sections).
- Inspect the evaluation's baselines, repeatability and memory-configuration assumptions, including what its results do and do not say about error correction (evaluation and discussion sections).
- Examine the paper's security/reliability distinction: an integrity risk in shared accelerator memory is not identical to a demonstrated cross-tenant privilege escalation or general-purpose GPU exploit.
- Review the proposed defensive directions at the level of memory integrity, error detection/correction, isolation and application robustness; assess their stated trade-offs without assuming all are experimentally validated in this paper.

## Comparison

[FPGAhammer](krautter-2018-fpgahammer.md) concerns power-delivery-induced timing faults in shared FPGA fabric. GPUHammer concerns DRAM read-disturbance bit flips in a discrete GPU's memory system. Despite the names, they rely on different physical mechanisms, attack surfaces and evaluation metrics; an FPGA fault rate is not a GPU DRAM bit-flip rate. The paper is also separate from [FHEmem](https://doi.org/10.48550/arXiv.2311.16293), which proposes a memory-centric accelerator architecture rather than reporting GPU Rowhammer susceptibility.

Reading state: Uploaded USENIX paper inspected for the GPU/memory scope, reported bit-flip observations, ML-model impact and mitigation discussion; no exploitation, independent reproduction or broader hardware generalization is claimed.

## Catalogue update, 4 November 2026

Seminar role: Core seminar literature.

[Publication page](https://www.usenix.org/conference/usenixsecurity25/presentation/lin-shaopeng) · [arXiv v2](https://arxiv.org/abs/2507.08166v2) · [arXiv DOI](https://doi.org/10.48550/arXiv.2507.08166) · [Public PDF](https://www.usenix.org/system/files/usenixsecurity25-lin-shaopeng.pdf) · [Author project](https://www.gpuhammer.com/) · [Author artifact](https://github.com/sith-lab/gpuhammer) · [Archived artifact](https://zenodo.org/records/15694512)

The USENIX citation record supplies no publication DOI. The linked arXiv DOI identifies the preprint.

### Summary and evidence

The USENIX abstract and author project report physical RowHammer faults in the tested NVIDIA RTX A6000 GDDR6 configuration and relate memory corruption to model integrity. The authors report up to eight bit flips across four tested banks and a single-bit model-impact example reducing ImageNet accuracy from about 80% to 0.1%.

### Place in the seminar

- Core, deep reading: compare GPU GDDR6 organization, access behavior and refresh constraints with CPU DRAM.
- Provide real-hardware disturbance evidence and a concrete AI-integrity consequence.

### Limits of the evidence

The tested GPU/configuration bounds the claim. Separate physical fault generation, model-impact evaluation and ECC trade-offs. The current arXiv record is v2 (16 September 2026); the existing uploaded-source note refers to the USENIX 2025 paper. No independent reproduction or full version comparison is claimed.

Source check (2026-11-04): USENIX publication/abstract, author project and current arXiv record; prior uploaded-paper notes preserved. Full reading remains unrecorded.

### Connections

[PRowhammer](shukla-2026-prowhammer.md) · [GPUThor](lin-2026-gputhor.md)

[Direction catalogue](index.md) · [Seminar overview](../seminar/README.md) · [Seminar reading note](../seminar/papers/lin-2025-gpuhammer.md)
