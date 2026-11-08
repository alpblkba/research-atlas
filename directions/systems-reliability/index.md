# Systems reliability and agentic SRE

A service can pass a health check and still fail for its callers. What evidence would convince me that a recovery action worked and left the service in a safe state? The two anchor papers are [SREGym](papers/clark-2026-sregym.md) and [STRATUS](papers/chen-2025-stratus.md); see sources for the records used.

## Read the papers against different axes

[SREGym](papers/clark-2026-sregym.md) is a benchmark/environment paper: live cloud-native stacks, injected faults, concurrent events/noise and varied failure modes. [STRATUS](papers/chen-2025-stratus.md) is an agent/system paper: specialized agents and a transactional no-regression safety objective. A harder benchmark is not itself a safer recovery policy, and an agent's success rate does not reveal whether the grading oracle misses regressions.

| Question | Why it matters |
|---|---|
| What exactly is the injected root cause? | Wrong ground truth or incomplete failure modeling distorts evaluation |
| Which logs/metrics can the agent see? | Observability affects diagnosis and may leak scenario answers |
| What is the success/rollback oracle? | An apparent service recovery may violate an invariant or regress later |
| Are correlated/noisy failures included? | Single-fault recovery is not enough to infer production reliability |

Reading exercise. Other systems-reliability papers can be added when their source and recommendation provenance are verified. [All directions](../index.md).
