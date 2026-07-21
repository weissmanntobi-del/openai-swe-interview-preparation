# Preparation Guide

## Do not prepare for a fictional universal interview loop

Software-engineering roles can differ substantially. A backend product engineer, a platform systems engineer, an inference engineer, and an enterprise AI engineer should not use identical preparation priorities.

Start with the current job description. Extract:

- primary users;
- expected programming languages;
- product versus infrastructure orientation;
- latency, scale, and reliability expectations;
- AI or ML depth;
- security and privacy requirements;
- ownership and collaboration expectations.

Then select the closest role map in this repository.

## Evidence hierarchy

Use this order when deciding what to study:

1. Current job description for the exact role.
2. Official interview guidance supplied by the company or recruiter.
3. Recruiter-provided preparation instructions.
4. Your demonstrated strengths and gaps.
5. Independent practice material such as this repository.
6. Anonymous online anecdotes only as weak, non-authoritative signals.

## Four interview modes

### Coding

The interviewer is evaluating more than syntax. Make your reasoning observable:

- clarify inputs and constraints;
- state invariants;
- describe the baseline;
- implement cleanly;
- test incrementally;
- respond constructively to changed constraints.

### System design

Avoid starting with a cloud-service inventory. Start with the user outcome and the riskiest mechanism.

A strong design answer should cover:

- workload;
- service objectives;
- data model;
- APIs;
- critical path;
- failure semantics;
- consistency;
- security;
- observability;
- deployment and rollback.

### Production judgment

Separate infrastructure health from product correctness. A system can be operationally “green” while producing unsafe, stale, expensive, or low-quality results.

### Behavioral judgment

Prepare examples showing:

- ownership;
- speed with protected invariants;
- constructive disagreement;
- recovery from error;
- working through ambiguity;
- measurable impact.

## Practice protocol

For each question:

1. Attempt it without notes.
2. Record the answer.
3. Score it using the repository rubric.
4. Identify the weakest two dimensions.
5. Repeat the same question with a changed constraint.
6. Write a short retrospective.

Breadth without revision creates familiarity, not interview readiness.
