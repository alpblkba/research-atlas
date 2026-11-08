# Papers: Memory systems

Memory-side disturbance papers currently live in [dependable computing](../../dependable-computing/papers/index.md) because they anchor the CDNC seminar. See [QPRAC](../../dependable-computing/papers/woo-2025-qprac.md) and [When Mitigations Backfire](../../dependable-computing/papers/woo-2025-when-mitigations-backfire.md). The papers below cover memory scheduling, interference and simulation.

## Direction-owned notes, added 2026-11-06

These notes are canonical in memory systems; RowHammer attack and mitigation papers stay in dependable computing and are linked from here.

### DRAM characterization, controllers and simulation

| Paper | Venue | Role |
|---|---|---|
| [Flipping bits in memory without accessing them](kim-2014-flipping-bits.md) | ISCA 2014 | original DRAM disturbance characterization |
| [Memory access scheduling](rixner-2000-memory-access-scheduling.md) | ISCA 2000 | origin of row-buffer-aware scheduling |
| [Ramulator 2.0](luo-2024-ramulator2.md) | IEEE Computer Architecture Letters 23(1) | simulator behind the WMB artifact |
| [DRAMSys4.0](steiner-2022-dramsys4.md) | International Journal of Parallel Programming 50(2) | independent TLM DRAM simulator |
| [Cerberus](kim-2026-cerberus.md) | ISCA 2026 | cross-layer ECC design |

### Interference, QoS and predictability

| Paper | Venue | Role |
|---|---|---|
| [MemGuard](yun-2013-memguard.md) | RTAS 2013 | per-core bandwidth regulation in software |
| [PREM](pellizzoni-2011-prem.md) | RTAS 2011 | phase-based predictable execution |
| [Denial-of-service attacks on shared cache](bechtel-2019-cache-dos.md) | RTAS 2019 | contention as an attack on partitioned caches |
| [MISE](subramanian-2013-mise.md) | HPCA 2013 | runtime slowdown estimation at the memory controller |
| [Heracles](lo-2015-heracles.md) | ISCA 2015 | datacenter colocation under isolation controls |

### CXL and processing in memory

| Paper | Venue | Role |
|---|---|---|
| [Demystifying CXL memory](sun-2023-demystifying-cxl.md) | MICRO 2023 | real CXL devices versus NUMA emulation |
| [Ambit](seshadri-2017-ambit.md) | MICRO 2017 | computation inside commodity DRAM |

[Direction overview](../index.md)
