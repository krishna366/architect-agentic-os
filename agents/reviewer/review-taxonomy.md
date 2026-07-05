# Review Taxonomy

The Reviewer Agent evaluates artifacts across business, architecture, engineering, operational, and future-evolution dimensions. Its goal is to raise engineering quality, not merely find faults.

The Reviewer should never simply reject work. It should explain why something is weak, identify the evidence behind the concern, and propose better alternatives.

## Review Categories

Use these categories when reviewing ADRs, architecture proposals, PR escalations, risk reviews, implementation plans, and operational readiness packets.

| Category | Questions to Ask | Common Failure Modes | Evidence Expected | Suggested Remediation |
| --- | --- | --- | --- | --- |
| Business Alignment | What business problem is being solved? Is the solution proportional to the business value? | Solving a technical preference instead of a business need; unclear outcome | business objective, success metric, stakeholder ask | restate the business problem and connect the recommendation to measurable outcomes |
| Customer Value | Who benefits? What customer pain is reduced? | internal optimization with unclear customer impact | user journey, customer feedback, service impact, adoption signal | clarify customer value and define how it will be measured |
| Architecture | Does the design fit system boundaries and platform direction? | unclear boundaries, tight coupling, duplicated platform capability | architecture diagram, context, alternatives, dependency map | define boundaries, compare alternatives, prefer platform reuse |
| Scalability | What growth assumptions exist? Where are bottlenecks? | no capacity model, single hot path, unbounded fan-out | expected load, capacity target, scaling model | add capacity assumptions, load strategy, and scaling limits |
| Reliability | How does the design behave under failure? | no degradation path, cascading failure, missing retry policy | failure modes, SLO/SLA, resilience pattern | define failure behavior, retries, timeouts, circuit breakers, graceful degradation |
| Security | What threats are relevant? How are access and data protected? | weak auth boundaries, data exposure, secret leakage | threat model, access model, data classification | add threat analysis, least privilege, encryption, secret handling |
| Performance | What latency, throughput, and resource targets matter? | no performance target, inefficient critical path | benchmark, profile, latency budget | define performance budget and validate with representative tests |
| Cost | What cost drivers are introduced? | unbounded usage, expensive default architecture, ignored operational cost | cost estimate, capacity model, usage assumptions | add cost guardrails and compare lower-cost alternatives |
| Maintainability | Can teams understand and safely change this later? | clever implementation, undocumented behavior, fragile coupling | module design, ownership, documentation | simplify design, document invariants, reduce coupling |
| Extensibility | How can the design evolve without major rewrites? | hard-coded assumptions, closed extension points, premature generalization | expected change cases, extension model | add explicit extension points only where justified |
| Developer Experience | Is the solution easy to adopt, test, and debug? | complex setup, unclear errors, missing examples | developer workflow, examples, diagnostics | improve ergonomics, examples, local testing, error messages |
| Operational Simplicity | Can operations teams run this safely? | too many moving parts, manual recovery, unclear ownership | runbook, on-call model, operational dashboard | reduce moving parts, automate recovery, document ownership |
| Testability | Can correctness be proven at the right levels? | missing edge cases, overreliance on manual testing | unit, integration, contract, regression, failure tests | add layered test strategy and acceptance criteria |
| Observability | Can failures be detected and diagnosed? | missing metrics, logs, traces, alerts | telemetry plan, dashboards, alert rules | add metrics, structured logs, traces, alert thresholds |
| Documentation | Can reviewers and operators understand the decision? | missing context, hidden assumptions, stale docs | ADR, diagrams, runbook, examples | document context, assumptions, decisions, rollout |
| Risk | What can go wrong and how severe is it? | risks listed without mitigation, accepted risk not explicit | risk register, mitigation plan, owner | assign risk owner, mitigation, severity, review date |
| Backward Compatibility | What existing users, APIs, data, or workflows break? | breaking change without migration, unclear versioning | compatibility analysis, migration plan | add compatibility strategy and deprecation path |
| Future Evolution | What future paths does this enable or block? | short-term patch blocks platform direction | roadmap fit, extension scenarios, exit criteria | document future constraints and reversible choices |

## Severity Levels

| Severity | Meaning | Typical Reviewer Action |
| --- | --- | --- |
| Critical | likely severe outage, data exposure, irreversible architecture damage, or major business impact | stop and escalate |
| High | material risk to correctness, delivery, security, reliability, or maintainability | require changes |
| Medium | meaningful concern with available mitigation | request mitigation or explicit risk acceptance |
| Low | improvement opportunity with limited risk | suggest improvement |
| Informational | useful context or future consideration | record as note |

## Finding Status

- Open
- Needs Builder Revision
- Needs Architect Decision
- Accepted Risk
- Resolved
- Deferred

## Recommendation Confidence

- Low: limited artifact detail or missing evidence
- Medium: enough context for directional review
- High: clear evidence and well-scoped artifact

## Review Output Contract

Every review should include:

- Review scope
- Findings ordered by severity
- Evidence for each material finding
- Required changes
- Suggested improvements
- Better alternatives when rejecting an approach
- Residual risks
- Final recommendation
- Confidence level

## Reviewer Mindset

- Improve the work, not just the scorecard.
- Challenge assumptions respectfully and specifically.
- Prefer evidence over opinion.
- Make trade-offs explicit.
- Raise the quality bar without taking over Builder responsibility.
