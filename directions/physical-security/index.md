# Physical security and faults

Two questions come up in my FPGA work. Can a mapped circuit leak information even if its logic is correct? Can activity elsewhere on the chip change the timing enough to produce a wrong result? I keep the measurements for those cases separate.

| Focus | Reading | What to extract |
|---|---|---|
| Mapping secure designs | [Meschkov et al. TCHES 2025](papers/meschkov-2025-secure-fpga-toolchain.md) | How modified LMDPL/WDDL primitives, masking and the toolchain relate to proofs and empirical leakage tests |
| Automated FPGA masking | [Müller et al. FPL 2023](papers/mueller-2023-automated-masking-fpga.md) | Which ASIC-oriented assumptions break or become expensive when mapped to LUTs and registers |
| Electrical fault scenario | [PWNN TCHES 2026](papers/xu-2026-pwnn.md) | How the authors define co-location, power integrity and fault observability; evaluate their evidence, not attack reproduction |
| Longer-term background | [Meschkov dissertation](papers/meschkov-2026-secure-reconfigurable-system.md) | Selective context after article-level questions are clear |

This direction connects to the [KIT/CDNC discussion](../dependable-computing/index.md) because physical constraints affect claims made by higher-level mitigations, not because every fault mechanism is Rowhammer. [All directions](../index.md).
