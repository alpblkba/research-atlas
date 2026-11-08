# Papers: Systems reliability

These are the sources I can return to for this direction. Each note records how far the source check went.

- [SREGym](clark-2026-sregym.md)
- [STRATUS](chen-2025-stratus.md)

## Failure studies and silent data corruption, added 2026-11-06

These notes give the benchmark papers above an empirical background: how production failures look, and how hardware faults surface as reliability incidents.

### Failure studies

| Paper | Venue | Role |
|---|---|---|
| [Gray failure](huang-2017-gray-failure.md) | HotOS 2017 | differential observability of failures |
| [Simple testing can prevent most critical failures](yuan-2014-simple-testing.md) | OSDI 2014 | empirical study of production failures |

### Silent data corruption

| Paper | Venue | Role |
|---|---|---|
| [Cores that don't count](hochschild-2021-cores-that-dont-count.md) | HotOS 2021 | silent data corruption in Google's fleet |
| [Silent data corruptions at scale](dixit-2021-sdc-at-scale.md) | arXiv preprint | silent data corruption in Meta's fleet |

[Direction overview](../index.md)
