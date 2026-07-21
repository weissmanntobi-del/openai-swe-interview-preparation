# Concurrency and Distributed Systems

## 11. At-Least-Once Consumer

A consumer updates a database and acknowledges a message. Design it so retries do not corrupt state.

Look for:
- transactional boundary;
- inbox or deduplication record;
- idempotent mutation;
- poison messages;
- replay strategy.

## 12. Outbox Relay

Design a transactional outbox and relay process.

Look for:
- atomic business write plus outbox write;
- polling or log-based relay;
- duplicate publication;
- ordering;
- retention and repair.

## 13. Distributed Lease Service

Design leases for background jobs across many workers.

Look for:
- fencing tokens;
- renewal;
- clock assumptions;
- split ownership;
- stale completion.

## 14. Fair Multi-Tenant Queue

Thousands of tenants submit jobs with different tiers and limits.

Look for:
- weighted fairness;
- per-tenant concurrency;
- starvation prevention;
- overload;
- admission control.

## 15. Distributed Rate Limiting

Enforce limits across regions.

Look for:
- strong versus approximate enforcement;
- local token allocation;
- hot keys;
- failure policy;
- abuse implications.

## 16. Cache Invalidation

A global service must propagate configuration changes quickly.

Look for:
- version numbers;
- push plus pull;
- stale tolerance;
- rollback;
- safe defaults.

## 17. Retry Storm

A dependency fails and thousands of clients retry simultaneously.

Look for:
- exponential backoff;
- jitter;
- retry budgets;
- circuit breaking;
- load shedding;
- recovery shaping.

## 18. Cross-Region State

A conversational service fails over between regions while preserving recent state.

Look for:
- replication lag;
- consistency requirements;
- session routing;
- data loss window;
- recovery reconciliation.
