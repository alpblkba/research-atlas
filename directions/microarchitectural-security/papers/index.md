# Papers: microarchitectural security

These records entered the catalogue on 2026-11-06. Each one names the source checked. The reading version is still open.

## Cache timing and transient execution

| Paper | Venue | Role |
|---|---|---|
| [FLUSH+RELOAD](yarom-2014-flush-reload.md) | USENIX Security 2014 | cache timing primitive |
| [Meltdown](lipp-2018-meltdown.md) | USENIX Security 2018 | out-of-order reads across the kernel boundary |
| [Spectre](kocher-2019-spectre.md) | IEEE S&P 2019 | speculation steered by trained predictors |
| [MIRAGE](saileshwar-2021-mirage.md) | USENIX Security 2021 | fully associative defense against eviction sets |

## Defenses and formal detection

| Paper | Venue | Role |
|---|---|---|
| [Speculative taint tracking (STT)](yu-2019-stt.md) | MICRO 2019 | hardware defense for speculatively accessed data |
| [Unique program execution checking (UPEC)](fadiheh-2019-upec.md) | DATE 2019 | formal leakage detection at RTL |
| [Helium](archer-2026-helium.md) | ISCA 2026 | quantified leakage with probabilistic guarantees |

## Apple Silicon

| Paper | Venue | Role |
|---|---|---|
| [PACMAN](ravichandran-2022-pacman.md) | ISCA 2022 | speculation against pointer authentication on M1 |
| [GoFetch](chen-2024-gofetch.md) | USENIX Security 2024 | data-dependent prefetcher leakage on Apple M-series |
| [Interrupt side channels on Apple Silicon](zhang-2026-apple-interrupt-side-channels.md) | ISCA 2026 | interrupt delivery as a side channel on macOS |

## Trusted execution and capabilities

| Paper | Venue | Role |
|---|---|---|
| [Keystone](lee-2020-keystone.md) | EuroSys 2020 | open TEE framework on RISC-V |
| [CHERIoT](amar-2023-cheriot.md) | MICRO 2023 | capability memory safety for microcontrollers |

## Related notes in other directions

[SonicBOOM](../../computer-architecture/papers/zhao-2020-sonicboom.md) · [TAGE branch prediction](../../computer-architecture/papers/seznec-2006-tage.md) · [Denial-of-service attacks on shared cache](../../memory-systems/papers/bechtel-2019-cache-dos.md) · [CLKSCREW](../../physical-security/papers/tang-2017-clkscrew.md) · [Plundervolt](../../physical-security/papers/murdock-2020-plundervolt.md) · [Thunderclap](../../operating-systems/papers/markettos-2019-thunderclap.md)

[Direction overview](../index.md)
