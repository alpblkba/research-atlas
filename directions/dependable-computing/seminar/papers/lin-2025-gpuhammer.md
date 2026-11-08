---
id: "lin-2025-gpuhammer"
title: "GPUHammer: Rowhammer Attacks on GPU Memories are Practical"
authors: ["Chris S. Lin", "Joyce Qu", "Gururaj Saileshwar"]
year: 2025
venue: "34th USENIX Security Symposium (USENIX Security '25), 5719–5738"
doi: null
source: "https://www.usenix.org/system/files/usenixsecurity25-lin-shaopeng.pdf"
status: "catalogued"
topics: ["memory-systems", "dependable-computing", "physical-security"]
added: "2026-11-04"
source_checked: "2026-11-04"
read_version: null
---
# GPUHammer

Seminar role: Core seminar literature, deep reading.

The [direction paper note](../../papers/lin-2025-gpuhammer.md) is the maintained source for metadata, verified links, summary, evidence and caveats. I keep the seminar questions here and use the direction note for citations.

## Summary and reading focus

The USENIX abstract and author project report physical RowHammer faults in the tested NVIDIA RTX A6000 GDDR6 configuration and relate memory corruption to model integrity. The authors report up to eight bit flips across four tested banks and a single-bit model-impact example reducing ImageNet accuracy from about 80% to 0.1%.

## Place in the seminar

- Core, deep reading: compare GPU GDDR6 organization, access behavior and refresh constraints with CPU DRAM.
- Provide real-hardware disturbance evidence and a concrete AI-integrity consequence.

## Evidence and caveats

The tested GPU/configuration bounds the claim. Separate physical fault generation, model-impact evaluation and ECC trade-offs. The current arXiv record is v2 (16 September 2026); the existing uploaded-source note refers to the USENIX 2025 paper. No independent reproduction or full version comparison is claimed.

[Source links and verification status](../../papers/lin-2025-gpuhammer.md#catalogue-update-4-november-2026) · [Full evidence note](../../papers/lin-2025-gpuhammer.md#summary-and-evidence)

Reading state: Catalogued as core; this entry does not mark a completed user full read.

[Seminar paper index](index.md) · [Seminar overview](../README.md) · [Direction catalogue](../../papers/index.md)
