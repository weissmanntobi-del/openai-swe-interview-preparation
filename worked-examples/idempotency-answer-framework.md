# Worked Example: Idempotent Request Processing

## Objective

Retries of one logical request must return a consistent result without repeating the protected external side effect.

## Important distinction

Idempotency is not merely “store the key.” The design must define behavior for:

- concurrent requests;
- same key with different payload;
- process crash;
- timeout after the side effect;
- expired records;
- permanently failed operations.

## Data model

Store:

- idempotency key;
- request fingerprint;
- state: in-progress, succeeded, failed;
- response metadata;
- creation and expiration timestamps;
- ownership or fencing token.

## Request path

1. Atomically create or read the idempotency record.
2. Reject key reuse with a different fingerprint.
3. If succeeded, return the stored result.
4. If in progress, wait, poll, or return a conflict according to the API contract.
5. Execute the side effect with its own idempotency mechanism where possible.
6. Atomically store the final result.

## Hard failure

If the system crashes after the external effect but before recording success, exactly-once behavior cannot be guaranteed unless the external system supports idempotency or reconciliation. State this explicitly.

## Tests

Include simultaneous duplicates, payload mismatch, crash injection, timeout, replay after success, and record expiry.
