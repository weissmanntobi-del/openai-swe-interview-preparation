# OpenAI-Oriented Software Engineering Interview Preparation

A rigorous, independent collection of **50 original practice questions** for software engineers preparing for roles involving backend systems, distributed infrastructure, developer platforms, applied AI, model serving, reliability, and product engineering.

> [!IMPORTANT]
> This repository is an independent educational resource. It is **not affiliated with, endorsed by, or sponsored by OpenAI**. It does not contain leaked, confidential, official, or guaranteed interview questions.

## What this repository helps you practise

The exercises are designed around durable engineering signals:

- problem framing before implementation;
- correct, readable, well-tested code;
- system design driven by invariants and failure modes;
- distributed systems, concurrency, queues, retries, and idempotency;
- AI-platform concerns such as evaluation, routing, streaming, inference, and retrieval;
- production judgment, incident response, security, and cost control;
- clear communication while requirements evolve.

## Start here

| Goal | Resource |
|---|---|
| Understand the repository | [Preparation guide](docs/PREPARATION_GUIDE.md) |
| Select questions for your target role | [Role maps](role-maps/) |
| Practise coding | [Coding questions](questions/01-coding.md) |
| Practise concurrency and distributed systems | [Distributed-systems questions](questions/02-distributed-systems.md) |
| Practise system design | [System-design questions](questions/03-system-design.md) |
| Practise AI infrastructure | [AI-platform questions](questions/04-ai-platform.md) |
| Practise incidents and operational judgment | [Reliability questions](questions/05-reliability.md) |
| Prepare behavioral stories | [Behavioral questions](questions/06-behavioral.md) |
| Review worked examples | [Worked examples](worked-examples/) |
| Run a focused sprint | [Seven-day plan](study-plans/7-day-plan.md) |
| Score a mock interview | [Interview scorecard](scorecards/interview-scorecard.md) |

## Question map

| Area | Questions |
|---|---:|
| Coding and practical implementation | 10 |
| Concurrency and distributed systems | 8 |
| Backend and platform system design | 10 |
| AI platform and model serving | 10 |
| Reliability and production incidents | 7 |
| Behavioral and hiring-manager judgment | 5 |
| **Total** | **50** |

## Representative questions

1. Implement a bounded, thread-safe TTL cache.
2. Build an idempotent request processor that survives crashes.
3. Design a fair multi-tenant work queue.
4. Design a resumable token-streaming API.
5. Design a model-routing gateway balancing quality, latency, and cost.
6. Diagnose stale citations in a production RAG system.
7. Respond to a partial regional inference-capacity failure.
8. Explain a technical decision that failed and how you corrected it.

## A better way to answer

For coding questions:

1. Clarify behavior and constraints.
2. State the invariant.
3. Implement the smallest correct version.
4. Test boundaries and failure cases.
5. Analyze complexity.
6. Explain production hardening.

For system-design questions:

1. Define the user outcome.
2. Quantify workload and service objectives.
3. State critical invariants.
4. Design the main request or data path.
5. Examine failure boundaries.
6. Add security, observability, and operations.
7. Defend trade-offs and identify unresolved risks.

For incident questions:

1. Stabilize.
2. Establish impact.
3. Segment the failure.
4. Mitigate safely.
5. Verify recovery.
6. Identify root cause.
7. Prevent recurrence.

## Public repository versus the complete playbook

This repository is a useful practice resource, not a substitute for a structured preparation system.

| Public repository | OpenAI Interview Playbook |
|---|---|
| 50 practice prompts | Deeper round-by-round preparation |
| Concise evaluation signals | Detailed strong-answer frameworks |
| Three worked examples | Broader walkthroughs and reference answers |
| One scorecard | Specialized rubrics and readiness checks |
| Seven-day plan | Full preparation strategy and sequencing |
| Community-friendly | Premium, structured self-study product |

### OpenAI Interview Playbook

For candidates who need deeper preparation, detailed answer frameworks, realistic mock material, evaluation rubrics, diagrams, take-home guidance, and structured study plans:

**[View the OpenAI Interview Playbook](https://tobiweissmann.gumroad.com/l/zefvek)**

The paid resource should be presented as a deeper preparation system—not as access to secret or guaranteed interview questions.

## Trust and sourcing

The repository separates three things clearly:

- **Official facts:** linked to current OpenAI sources.
- **Original practice material:** authored for preparation and labeled as such.
- **Interpretation:** role-oriented engineering themes inferred from public job descriptions, not claims about a specific interview.

See [Sources and methodology](docs/SOURCES_AND_METHODOLOGY.md).

## Suggested GitHub metadata

**Repository name**

```text
openai-swe-interview-preparation
```

**Description**

```text
50 original coding, distributed-systems, system-design, AI-platform, reliability, and behavioral questions for OpenAI-oriented software engineering interview preparation.
```

**Topics**

```text
software-engineering-interview
openai-interview
coding-interview
system-design
distributed-systems
backend-engineering
platform-engineering
ai-infrastructure
llmops
reliability-engineering
```

## Responsible contribution policy

Contributions are welcome, but this repository does not accept leaked, confidential, or memorized interview content. Submit only original educational exercises or improvements to existing material.

## License

Original repository content is available under the [CC BY-NC 4.0 license](LICENSE.md). Commercial reuse and resale are not permitted without written permission.

## Author

Created by **Tobias Weissmann**.

