# Papers: Accelerators

These are the sources I can return to for this direction. Each note records how far the source check went.

- [FHEmem](zhou-2023-fhemem.md) · Zhou, M., et al. (2023). *FHEmem: A Processing In-Memory Accelerator for Fully Homomorphic Encryption*. arXiv preprint. [doi:10.48550/arXiv.2311.16293](https://doi.org/10.48550/arXiv.2311.16293).
- [HEAWS](turan-2020-heaws.md) · Turan, F., Sinha Roy, S., & Verbauwhede, I. (2020). *HEAWS: An Accelerator for Homomorphic Encryption on the Amazon AWS FPGA*. IEEE Transactions on Computers, 69(8), 1185–1196. [doi:10.1109/TC.2020.2988765](https://doi.org/10.1109/TC.2020.2988765).
- [MemFHE](gupta-2024-memfhe.md) · Gupta, S., Cammarota, R., & Šimunić Rosing, T. (2024). *MemFHE: End-to-End Computing with Fully Homomorphic Encryption in Memory*. ACM Transactions on Embedded Computing Systems, 23(2). [doi:10.1145/3569955](https://doi.org/10.1145/3569955).
- [SoK: Fully Homomorphic Encryption Accelerators](zhang-2024-sok-fhe-accelerators.md) · Zhang, J., et al. (2024). *SoK: Fully Homomorphic Encryption Accelerators*. ACM Computing Surveys, 56(12), Article 316. [doi:10.1145/3676955](https://doi.org/10.1145/3676955).

## Architecture and methodology literature, added 2026-11-06

These notes widen the direction beyond the archived FHE work to general accelerator design and evaluation.

### Arrays, dataflow and evaluation

| Paper | Venue | Role |
|---|---|---|
| [Why systolic architectures?](kung-1982-systolic.md) | IEEE Computer 15 | original systolic array argument |
| [Tensor Processing Unit](jouppi-2017-tpu.md) | ISCA 2017 | production int8 systolic accelerator |
| [Eyeriss](chen-2016-eyeriss.md) | ISCA 2016 | dataflow taxonomy by operand reuse |
| [Timeloop](parashar-2019-timeloop.md) | ISPASS 2019 | mapping-aware accelerator evaluation |
| [Gemmini](genc-2021-gemmini.md) | DAC 2021 | accelerator evaluated inside a full SoC |

### Network data planes

| Paper | Venue | Role |
|---|---|---|
| [Forwarding metamorphosis (RMT)](bosshart-2013-rmt.md) | SIGCOMM 2013 | programmable switch pipeline in hardware |

[Direction overview](../index.md)
