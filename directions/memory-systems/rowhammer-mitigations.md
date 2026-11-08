# Rowhammer mitigation: protection, timing and cost

## Problem map

A controller can keep activations below a disturbance threshold and still reveal which requests triggered mitigation. I want to evaluate those properties separately. The [QPRAC paper](../dependable-computing/papers/woo-2025-qprac.md) examines practical, secure servicing of pending PRAC mitigations. [When Mitigations Backfire](../dependable-computing/papers/woo-2025-when-mitigations-backfire.md) shows that PRAC's activity-dependent Alert Back-Off and Refresh Management behavior can itself create timing channels and proposes activity-independent Timing-Based RFMs (TPRAC). This framing comes from the authors' abstracts and conference paper, not a completed independent review.

| Dimension | QPRAC (HPCA 2025) | When Mitigations Backfire (ISCA 2025) |
|---|---|---|
| Problem emphasized | Securely schedule row-level mitigation without impractical oracular knowledge | PRAC-triggered mitigation timing exposes activation behavior |
| Mechanism to inspect | Priority service queue; proactive REF and opportunistic RFM mitigation | PRACLeak characterization; TPRAC with periodic Timing-Based RFMs |
| Security question | Is Rowhammer protection maintained under adversarial activation patterns? | Does RFM timing leak information about victim activity? |
| Cost question | Queue state, ABO interruptions and slowdown | Periodic refresh overhead and elimination of timing variation |
| Comparison hazard | Author-reported slowdown under the paper's benign workloads | Author-reported slowdown under different policy/threshold/workload settings |

## The comparison we actually need

Do not compare headline slowdowns as if they were on the same baseline. Extract the Rowhammer threshold, PRAC configuration, preventive refresh frequency, workload traces, performance metric and security assumption from each paper. Decide whether timing-channel resistance is explicitly covered before calling a design secure in that dimension. See the comparison worksheet.

## Seminar boundary

This note supports a literature question, not a new attack or a live simulator. Experimental work, if any, lives in a separate repository. [CDNC seminar](../dependable-computing/seminar/README.md).
