# Memory systems

Current focus: [Architectural Rowhammer mitigations](rowhammer-mitigations.md). A secondary thread asks what large encrypted workloads spend on data movement: [FHEmem](../accelerators/papers/zhou-2023-fhemem.md) and [FHE data movement](../accelerators/fhe-data-movement.md).

## Open questions

- What does the DRAM controller observe, and which mitigation decisions live inside DRAM rather than in the host?
- How do activation counters, queued mitigations and RFM commands affect shared-channel occupancy and access latency?
- Does the reported overhead include the relevant operating point, e.g., Rowhammer threshold and workload mix?
- Which results depend on a specific assumed DRAM interface, rather than generalizing to every DDR generation?

This direction is broader than Rowhammer; caches, CXL, memory-tiering and accelerator data movement can enter when a concrete source warrants it. [All directions](../index.md).
