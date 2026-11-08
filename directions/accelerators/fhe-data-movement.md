# Data movement in FHEmem and HEAWS

## Where the work goes

[FHEmem](papers/zhou-2023-fhemem.md) targets FHE's large working set and long-bitwidth operations with processing close to DRAM storage; its author abstract stresses both computation and complex data movement. [HEAWS](papers/turan-2020-heaws.md) maps FV homomorphic operations onto an AWS FPGA with parallel coprocessors and a high-bandwidth host-device interface. The HEAWS paper abstract explicitly discusses 512-bit XDMA transfers and the off-chip feeding strategy. Those are different architectural boundaries and different homomorphic-encryption schemes.

| Comparison axis | FHEmem | HEAWS |
|---|---|---|
| Primary architectural lens | Near-memory / near-mat compute and data reuse | FPGA coprocessor parallelism, on-chip storage and host-device communication |
| Scheme in the examined materials | CKKS is central in the preserved seminar discussion; verify each evaluated configuration in the paper | FV exact-arithmetic scheme in the source abstract |
| Likely transfer boundary to inspect | Movement among DRAM structures, near-mat units and transformations | Host/FPGA via XDMA plus on-/off-chip storage |
| What not to do | Claim all speedups generalize to every FHE scheme | Compare reported multiplications/s with FHEmem results without matching parameters |

## Historical material already available

The old presentation had sections on FHE workload anatomy, NTT, BConv, key switching, near-mat units, mapping and an FHEmem-versus-HEAWS slide. Those are useful starting points, not verified conclusions. Inspect the [available presentations](slides/README.md), report source and [provenance](fhe-seminar/provenance.md) locally before reusing numbers or diagrams. The earlier concise Markdown draft is missing from this vault snapshot.

The complete preserved seminar export and source variants are also available. Its embedded Overleaf version matches the earlier archived `main.tex`, while the outer exported `main.tex` is different; no version has been silently promoted to the canonical text.

## One concrete reconciliation task

Pick the slide comparing FHEmem and HEAWS. For each metric, record scheme, ciphertext parameters, NTT/key-switching phase, host transfers, timing boundary and comparison baseline. If the setups differ, present a qualitative architecture comparison rather than inventing a normalized performance ranking. Worksheet.
