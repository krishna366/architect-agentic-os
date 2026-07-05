# Reviewer Agent Outputs

## Primary Outputs

- architecture review
- ADR review
- PR review escalation
- risk review
- reviewer-to-builder packet
- reviewer-to-strategist packet

## Output Contract

Every output must include:

- status: Draft / Needs Review / Approved / Archived
- review scope
- findings ordered by severity
- required changes
- suggested improvements
- risks
- confidence level
- final recommendation
- decisions needed

## Final Recommendation Values

- Approve
- Approve with Conditions
- Request Changes
- Needs Discussion
- Escalate

## Review Checklist

- [ ] Human-auditable
- [ ] Findings are actionable
- [ ] No confidential raw context
- [ ] Facts and assumptions are separated
- [ ] Handoff packet is used when another agent must act
