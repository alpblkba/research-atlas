# Papers: operating systems

These records entered the catalogue on 2026-11-06. Each one names the source checked. The reading version is still open.

## Kernel structure, IPC and verification

| Paper | Venue | Role |
|---|---|---|
| [Improving IPC by kernel design](liedtke-1993-improving-ipc.md) | SOSP 1993 | kernel design around fast IPC |
| [SeL4](klein-2009-sel4.md) | SOSP 2009 | scope and assumptions of a verified kernel |
| [The Multikernel](baumann-2009-multikernel.md) | SOSP 2009 | message passing instead of shared kernel state |
| [Verus](lattuada-2024-verus.md) | SOSP 2024 | SMT-based verification of Rust systems code |

## Virtualization

| Paper | Venue | Role |
|---|---|---|
| [Formal requirements for virtualizable architectures](popek-1974-virtualizable-architectures.md) | Communications of the ACM 17 | ISA conditions for virtualization |
| [Memory resource management in VMware ESX Server](waldspurger-2002-esx-memory.md) | OSDI 2002; ACM SIGOPS Operating Systems Review 36 | hypervisor memory techniques, including page sharing |
| [Dune](belay-2012-dune.md) | OSDI 2012 | virtualization hardware reused for process isolation |

## Virtual memory and tiering

| Paper | Venue | Role |
|---|---|---|
| [Efficient virtual memory for big memory servers (direct segments)](basu-2013-direct-segments.md) | ISCA 2013 | translation overhead and a minimal hardware fix |
| [EMT](chai-2025-emt.md) | OSDI 2025 | Linux support for new translation hardware |
| [TPP](maruf-2023-tpp.md) | ASPLOS 2023 | kernel page placement for CXL tiers |
| [PagedAttention](kwon-2023-pagedattention.md) | SOSP 2023 | paging applied to LLM KV caches |

## Kernel bypass, interference and I/O

| Paper | Venue | Role |
|---|---|---|
| [The eXpress Data Path (XDP)](hoiland-jorgensen-2018-xdp.md) | CoNEXT 2018 | programmable packet processing inside the kernel |
| [Caladan](fried-2020-caladan.md) | OSDI 2020 | interference control by fast core reallocation |
| [Thunderclap](markettos-2019-thunderclap.md) | NDSS 2019 | DMA attacks against IOMMU usage |

## Related notes in other directions

[MemGuard](../../memory-systems/papers/yun-2013-memguard.md) · [Demystifying CXL memory](../../memory-systems/papers/sun-2023-demystifying-cxl.md) · [Meltdown](../../microarchitectural-security/papers/lipp-2018-meltdown.md) · [CHERIoT](../../microarchitectural-security/papers/amar-2023-cheriot.md) · [Keystone](../../microarchitectural-security/papers/lee-2020-keystone.md)

[Direction overview](../index.md)
