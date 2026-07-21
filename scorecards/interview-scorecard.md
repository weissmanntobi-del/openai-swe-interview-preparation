# Interview Scorecard

Score each dimension from 1 to 5.

| Dimension | 1 | 3 | 5 |
|---|---|---|---|
| Problem framing | Starts immediately | Clarifies main scope | Reframes outcome, constraints, and risks |
| Correctness | Happy path only | Correct baseline | Explicit invariants and boundary behavior |
| Code quality | Difficult to follow | Reasonably structured | Small, testable, adaptable components |
| Testing | Examples only | Main cases covered | Deterministic boundary, failure, and concurrency tests |
| Complexity | Missing | Basic analysis | Connects complexity to constraints and alternatives |
| Architecture | Generic boxes | Coherent flow | Prioritizes risky mechanisms and defends trade-offs |
| Reliability | “Add retries” | Handles common failures | Distinguishes retryable, unsafe, and degraded states |
| Security | Mentions authentication | Defines controls | Enforceable isolation, revocation, and auditability |
| AI quality | Vague testing | Relevant metrics | Datasets, graders, release gates, monitoring, rollback |
| Communication | Final answer only | Explains main reasoning | Exposes assumptions, uncertainty, and decisions |
| Operational judgment | Limited | Basic observability | Recovery criteria, ownership, capacity, and rollout |
| Senior judgment | Overbuilds or hand-waves | Reasonable choices | Protects invariants and scopes deliberately |

## Interpretation

- 52–60: strong mock performance;
- 43–51: credible, with targeted weaknesses;
- 32–42: inconsistent under pressure;
- below 32: rebuild fundamentals and repeat fewer questions deeply.

This score is diagnostic, not predictive.
