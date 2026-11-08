---
id: "kwon-2023-pagedattention"
title: "Efficient Memory Management for Large Language Model Serving with PagedAttention"
authors: ["Woosuk Kwon", "Zhuohan Li", "Siyuan Zhuang", "Ying Sheng", "Lianmin Zheng", "Cody Hao Yu", "Joseph E. Gonzalez", "Hao Zhang", "Ion Stoica"]
year: 2023
venue: "SOSP 2023, pp. 611-626"
doi: "10.1145/3600006.3613165"
source: "https://doi.org/10.1145/3600006.3613165"
status: "catalogued"
topics: ["operating-systems", "accelerators"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# PagedAttention

[Publication DOI](https://doi.org/10.1145/3600006.3613165) · [Direction catalogue](index.md)

## Reading focus

PagedAttention manages the KV cache in blocks and uses a mapping table to find them. Fragmentation and copy-on-write make this a virtual-memory question inside an accelerator workload.

- An entry into AI serving systems that does not require starting from model internals.

Reading tier: optional.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the OpenAlex record.

OpenAlex abstract: PagedAttention is a memory-management method inspired by OS virtual memory paging that reduces KV-cache waste in LLM serving and raises throughput.

## Questions for the full paper

- Which OS concepts map directly (pages, page tables, sharing), and which do not?
- How much fragmentation do existing systems show, and how much does paging remove?
- Where does the GPU kernel pay for the extra indirection?

## Connections

[Efficient virtual memory for big memory servers (direct segments)](basu-2013-direct-segments.md) · [TPP](maruf-2023-tpp.md) · [Tensor Processing Unit](../../accelerators/papers/jouppi-2017-tpu.md)
