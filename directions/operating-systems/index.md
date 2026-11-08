# Operating systems

My starting point is what the kernel needs from the hardware, and what each hardware mechanism forces the kernel to do. It covers kernel structure and IPC, virtualization, virtual memory and memory tiering, kernel bypass and interference control, DMA and I/O protection, and systems verification. Leakage mechanisms below the ISA live in [microarchitectural security](../microarchitectural-security/index.md) even when the kernel is the victim.

## Open questions

- Which hardware feature does a kernel mechanism depend on, and what changes on Arm, x86 or RISC-V?
- Where should interference be controlled: partitioning in hardware, regulation in the kernel, or fast reallocation by a user-level scheduler?
- What does a proof or verifier cover in a kernel, and what does it assume about the hardware?
- How does CXL tiering change page placement, and can the evidence be trusted when CXL is emulated?

[Papers](papers/index.md) · [All directions](../index.md)
