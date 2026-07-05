# Reviewer Agent Inputs

## Accepted Inputs

- ADR draft
- architecture proposal
- implementation plan
- PR summary or diff summary
- risk register item
- test plan
- operational readiness packet
- Builder-to-Reviewer packet
- sanitized project context

## Input Processing

For every input, extract:

- source
- date
- artifact type
- review scope
- decision under review
- claimed outcome
- assumptions
- risks
- evidence provided
- missing evidence
- review recommendation needed

## Input Quality Checklist

- [ ] Review scope is clear
- [ ] Artifact status is marked
- [ ] Confidential raw context is excluded or explicitly approved
- [ ] Acceptance criteria or decision criteria are available
- [ ] Evidence is linked or summarized

## Example

Input: "Review this ADR for adopting event-driven integration."

Process as:

- Artifact type: ADR
- Review scope: architecture, reliability, operational readiness
- Needed output: ADR review with required changes and final recommendation
