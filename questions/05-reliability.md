# Reliability and Production Incidents

## 39. P99 Latency Regression

Average latency is stable, but P99 doubled after a release.

Segment by model, region, token length, queue time, batch size, cold loads, and dependency latency.

## 40. Duplicate External Actions

Retries caused duplicate notifications and charges.

Separate delivery semantics, idempotency, acknowledgement timing, transaction boundaries, and reconciliation.

## 41. Growing Queue, Idle Workers

Queue depth grows while worker CPU remains low.

Investigate dependency saturation, polling, leases, partitions, concurrency controls, poison jobs, and rate limiting.

## 42. Stale RAG Citation

A confident answer cites a superseded policy.

Investigate versioning, effective dates, permissions, retrieval filters, reranking, citation entailment, abstention, and evaluation gaps.

## 43. Partial Regional Inference Failure

A region loses substantial serving capacity during peak demand.

Decide failover, load shedding, model fallback, tier prioritization, state consistency, communication, and recovery validation.

## 44. Cost Spike Without Traffic Growth

Inference cost rises sharply while request count is stable.

Investigate token growth, retries, routing, cache misses, agent loops, tool amplification, configuration changes, and accounting errors.

## 45. Evaluation Passed, Production Quality Fell

Offline evaluation improved, but user satisfaction declined after launch.

Investigate dataset representativeness, metric gaming, segment regressions, online behavior, feedback loops, instrumentation, and rollback criteria.
