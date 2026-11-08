# Computer architecture

I want to understand where performance and correctness come from inside a core and its memory hierarchy, and how a claim about either is measured. It covers processor microarchitecture, prediction, memory ordering, open RISC-V platforms, simulation methodology and formal ISA models. DRAM and memory controllers live in [memory systems](../memory-systems/index.md); security consequences of microarchitecture live in [microarchitectural security](../microarchitectural-security/index.md).

## Open questions

- Which structures in an out-of-order core hold speculative state, and what does a squash actually restore?
- When is a reported IPC or speedup comparable: same ISA, same memory system, same simulator or silicon?
- What does an in-order core such as [rv32i-mla](https://github.com/alpblkba/rv32i-mla) need before branch prediction pays off, and how would the gain be measured?
- Which properties can a formal ISA model check against RTL, and which need a different method?

[Papers](papers/index.md) · [All directions](../index.md)
