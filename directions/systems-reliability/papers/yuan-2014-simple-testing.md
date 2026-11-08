---
id: "yuan-2014-simple-testing"
title: "Simple Testing Can Prevent Most Critical Failures: An Analysis of Production Failures in Distributed Data-Intensive Systems"
authors: ["Ding Yuan", "Yu Luo", "Xin Zhuang", "Guilherme Renna Rodrigues", "Xu Zhao", "Yongle Zhang", "Pranay U. Jain", "Michael Stumm"]
year: 2014
venue: "OSDI 2014, pp. 249-265"
doi: null
source: "https://www.usenix.org/conference/osdi14/technical-sessions/presentation/yuan"
status: "catalogued"
topics: ["systems-reliability"]
added: "2026-11-06"
source_checked: "2026-11-06"
read_version: null
---
# Simple testing can prevent most critical failures

[Source](https://www.usenix.org/conference/osdi14/technical-sessions/presentation/yuan) · [Direction catalogue](index.md)

## Reading focus

Yuan et al. work backward from production failures to small reproductions and error-handling paths. Those cases give me something concrete against which to judge a fault-injection benchmark.

- Shows the method behind failure studies (sampling, classification, a derived checker), useful when judging how realistic SREGym scenarios are.

Reading tier: core.

## Source record

Source check by agent, 2026-11-06: metadata and abstract from the USENIX presentation page.

USENIX abstract: 198 user-reported failures in Cassandra, HBase, HDFS, Hadoop MapReduce and Redis were analyzed; almost all reproduce on three or fewer nodes, logs usually suffice for diagnosis, and a static checker (Aspirator) derived from the catastrophic cases would have prevented over 30% of them and found 143 bugs and bad practices.

## Questions for the full paper

- How were the failures sampled, and what bias does that introduce?
- Which error-handling patterns caused the catastrophic failures?
- How do the findings carry over to Kubernetes-based microservice failures?

## Connections

[Gray failure](huang-2017-gray-failure.md) · [SREGym](clark-2026-sregym.md)
