# Compilers and runtimes

I want to follow the assumptions that survive each step from source code to a running system. [LLVM](papers/lattner-2004-llvm.md), [MLIR](papers/lattner-2021-mlir.md) and [Alive2](papers/lopes-2021-alive2.md) cover intermediate representations, lowering and checks on transformations. [TensorFlow Lite Micro](papers/david-2021-tflm.md) brings the question down to the layout of an activation arena in SRAM.

In FPGA mapping, preserving the logical output is only part of the job. [Meschkov et al. 2025](../physical-security/papers/meschkov-2025-secure-fpga-toolchain.md) studies a reconfigurable fabric and mapping toolchain designed with physical protection in mind. [Müller et al. 2023](../physical-security/papers/mueller-2023-automated-masking-fpga.md) looks at automatically generated masked FPGA designs. Which security assumptions survive optimization, retiming and placement? Which properties have formal support, and which depend on measurements?

[Nix](papers/dolstra-2004-nix.md), [reproducible builds](papers/lamb-2022-reproducible-builds.md) and [Thompson's compiler example](papers/thompson-1984-trusting-trust.md) cover the inputs and trust assumptions behind a binary. I keep those questions alongside compilation because source-level reasoning alone does not identify the artifact I actually run.

[Paper catalogue](papers/index.md) · [All directions](../index.md)
