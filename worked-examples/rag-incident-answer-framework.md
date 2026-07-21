# Worked Example: Stale RAG Citation Incident

## Stabilize

- Identify affected tenants, workflows, and policy domains.
- Disable or constrain the risky answer path.
- Prefer abstention or escalation over confident unsupported answers.
- Preserve evidence for investigation.

## Segment the pipeline

Check each boundary separately:

1. source ingestion;
2. document versioning;
3. permissions and metadata;
4. retrieval;
5. reranking;
6. prompt construction;
7. generation;
8. citation validation;
9. product presentation.

## Likely failure classes

- current document never ingested;
- superseded document not marked inactive;
- effective-date filter missing;
- permissions incorrect;
- lexical match favored old wording;
- citation validator checked existence, not support;
- evaluation dataset lacked version-conflict cases.

## Recovery criteria

Do not declare recovery merely because error rates are low. Verify:

- current document retrieved;
- obsolete document suppressed appropriately;
- citations support the generated claim;
- known incident examples pass;
- representative tenant segments pass;
- monitoring detects recurrence.

## Prevention

Add temporal metadata, document lifecycle rules, retrieval filters, entailment checks, abstention thresholds, adversarial fixtures, and release gates.
