# Papers: Compilers and runtimes

The current cross-listed architecture papers are [secure FPGA/toolchain](../../physical-security/papers/meschkov-2025-secure-fpga-toolchain.md) and [automated FPGA masking](../../physical-security/papers/mueller-2023-automated-masking-fpga.md), retained under physical security. The compiler and runtime papers below have their own records here.

## Direction-owned notes, added 2026-11-06

These notes add software compiler, runtime and supply chain sources alongside the cross-listed FPGA toolchain papers above.

### Compiler infrastructure and correctness

| Paper | Venue | Role |
|---|---|---|
| [LLVM](lattner-2004-llvm.md) | CGO 2004 | compiler IR and pass infrastructure |
| [MLIR](lattner-2021-mlir.md) | CGO 2021 | multi-level IR for domain-specific lowering |
| [Alive2](lopes-2021-alive2.md) | PLDI 2021 | translation validation of compiler optimizations |

### Embedded runtimes

| Paper | Venue | Role |
|---|---|---|
| [TensorFlow Lite Micro](david-2021-tflm.md) | MLSys 2021 | MCU inference runtime with a planned tensor arena |

### Toolchain trust and reproducibility

| Paper | Venue | Role |
|---|---|---|
| [Reflections on trusting trust](thompson-1984-trusting-trust.md) | Communications of the ACM 27(8) | trust in compiled artifacts |
| [Reproducible builds](lamb-2022-reproducible-builds.md) | IEEE Software 39(2) | verifying binaries against source |
| [Nix](dolstra-2004-nix.md) | LISA 2004 | content-addressed deployment |

[Direction overview](../index.md)
