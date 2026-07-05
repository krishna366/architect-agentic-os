# Opportunity Scoring

The Explorer Agent uses this framework to evaluate new technologies, research papers, products, open-source projects, standards, and architectural ideas without chasing trends.

The goal is to generate a prioritized innovation backlog of ideas that can become architecture proposals, reusable frameworks, enterprise platform capabilities, or focused PoCs.

## Scoring Scale

Score each dimension from 1 to 5.

- 1: weak or unfavorable
- 2: limited
- 3: plausible
- 4: strong
- 5: exceptional

## Scoring Dimensions

| Dimension | What to Evaluate | High Score Means |
| --- | --- | --- |
| Strategic Relevance | alignment with long-term architecture direction | clearly advances a durable strategic theme |
| Customer Value | customer or user problem addressed | solves a meaningful pain point |
| Business Impact | revenue, cost, speed, risk, or capability impact | material business outcome is plausible |
| Technical Novelty | meaningful new capability or pattern | creates a new option, not just a minor variation |
| Implementation Complexity | difficulty of prototype and adoption | feasible with controlled effort |
| Time to Prototype | speed to learn through a small experiment | useful signal can be produced quickly |
| Ecosystem Maturity | docs, community, vendor stability, examples | stable enough to evaluate responsibly |
| Standards Alignment | fit with open standards or accepted protocols | avoids avoidable proprietary lock-in |
| Competitive Advantage | differentiation or market relevance | creates meaningful strategic advantage |
| Learning Value | value of the learning even if not adopted | teaches an important architecture lesson |
| Reusability | potential to become a reusable capability | useful across multiple teams or domains |
| Long-Term Importance | likelihood the idea matters over years | durable trend rather than short-lived hype |
| Risk | security, reliability, compliance, delivery risk | manageable and explicit |
| Cost | financial and operational cost | low or justified by value |
| Adoption Probability | likelihood teams can realistically adopt it | adoption path is credible |

## Opportunity Score

Opportunity Score:

Strategic Relevance + Customer Value + Business Impact + Technical Novelty + Implementation Complexity + Time to Prototype + Ecosystem Maturity + Standards Alignment + Competitive Advantage + Learning Value + Reusability + Long-Term Importance + Risk + Cost + Adoption Probability

Maximum Score: 75

## Recommendation Bands

- 61-75: Production Candidate after validation
- 49-60: Pilot candidate
- 37-48: Prototype candidate
- 25-36: Research or watch
- 15-24: Ignore unless new evidence appears

## Recommendation Values

Every opportunity should receive one recommendation:

- Ignore: not relevant, too risky, or too weak
- Watch: interesting but immature or poorly timed
- Research: worth deeper investigation before hands-on work
- Prototype: worth a small technical experiment
- Pilot: worth limited real-world use with guardrails
- Production Candidate: strong validated candidate for broader adoption

## Prioritization Rules

1. Reward ideas that solve meaningful problems.
2. Reward ideas that can become architecture proposals, reusable frameworks, or enterprise platform capabilities.
3. Prefer standards-aligned ideas over proprietary one-offs.
4. Prefer learning-rich prototypes over vague exploration.
5. Penalize fashionable ideas with weak evidence.
6. Penalize ideas that add operational burden without clear value.
7. Penalize ideas that create lock-in without strategic reason.
8. Consider business timing, not only technical merit.

## Required Opportunity Notes

- Opportunity:
- Source References:
- Problem Solved:
- Target User or Team:
- Score:
- Recommendation:
- Confidence Level:
- Key Evidence:
- Main Assumption:
- Main Risk:
- Prototype Path:
- Success Metric:
- Next Review Date:

## Innovation Backlog Fields

Use these fields when adding an item to the innovation backlog:

- Backlog ID:
- Theme:
- Opportunity:
- Score:
- Recommendation:
- Owner:
- Review Date:
- Current Status:
- Next Action:
