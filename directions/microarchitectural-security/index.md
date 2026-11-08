# Microarchitectural security

I keep coming back to when an optimization below the ISA breaks a guarantee stated at or above it. It covers cache timing channels, transient execution attacks and defenses, formal leakage detection, Apple Silicon reverse engineering, trusted execution and capability hardware. Electrical faults and power side channels stay in [physical security](../physical-security/index.md) and DRAM disturbance in [dependable computing](../dependable-computing/index.md); the three share the theme of an effect crossing an abstraction boundary but rely on different evidence.

## Open questions

- Which architectural guarantee is violated, by which microarchitectural state, and through which observable channel?
- Is a defense evaluated in a simulator, on RTL or on silicon, and under which threat model?
- Can the leakage be found formally before tape-out, and does the method scale to an out-of-order core?
- Which results depend on undocumented vendor behavior, and how was that behavior reverse-engineered?

[Papers](papers/index.md) · [All directions](../index.md)
