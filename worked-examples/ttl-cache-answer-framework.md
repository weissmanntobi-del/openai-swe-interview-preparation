# Worked Example: TTL Cache Answer Framework

This is an answer framework, not a complete implementation.

## Clarify

- Is capacity bounded?
- Does expiration use a monotonic clock?
- Is lazy cleanup sufficient?
- Is concurrent access required?
- What should `get` return for expired entries?
- Is eviction LRU, FIFO, or arbitrary?

## Core invariant

A successful `get(key)` must never return an entry whose expiration time is less than or equal to the current monotonic time.

## Baseline

Use a hash map storing value and expiration timestamp. On `get`, compare expiration with the injected clock and remove expired entries lazily.

## Concurrency

For a first correct version, protect map and eviction metadata with one lock. Explain that a single lock is intentionally simple and may later be replaced with sharding or a production cache.

## Deterministic tests

- value before expiration;
- value exactly at expiration;
- overwrite resets expiration;
- delete;
- capacity eviction;
- concurrent read/write safety;
- no real sleeping—advance a fake clock.

## Hardening

Add memory accounting, metrics, background cleanup, bounded cleanup work, and operational limits. For multi-node use, clarify whether local caches may diverge and how invalidation works.
