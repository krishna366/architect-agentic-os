# Architect Agentic OS

Architect Agentic OS is a lightweight operating model for running a personal and team-oriented AI agent system around architecture work, project execution, technical review, innovation discovery, executive communication, and long-term career growth.

The goal is not to create one all-knowing assistant. The goal is to create a structured set of agents with clear roles, clean context boundaries, auditable handoffs, and reusable professional character.

## Why this exists

Senior architects often operate across multiple projects, stakeholders, documents, decisions, risks, and future-facing ideas. Without structure, AI assistants can become noisy, context-polluted, and hard to trust.

This repository defines a disciplined agent system where:

- Project-specific agents gather current project signals.
- Builder agents convert project context into architecture and execution artifacts.
- Reviewer agents challenge assumptions, risks, and design quality.
- Explorer agents research future opportunities and emerging ideas.
- Strategist agents translate technical work into executive narratives.
- Navigator agents support long-term career direction using sanitized personal inputs.

## Core Principle

Project context is temporary. Professional character is portable.

This system separates:

- **Project memory**: specific to a company, project, codebase, roadmap, or team.
- **Professional memory**: reusable principles, review standards, architecture judgment, communication style, and leadership philosophy.

Only professional memory should be carried across jobs or organizations.

## Agent Types

### Project Agent

Maintains current understanding of a specific project.

Responsibilities:

- Track project goals, open decisions, blockers, risks, and recent changes.
- Summarize relevant inputs from documents, tickets, code, meetings, and discussions.
- Produce human-auditable task packets for Builder agents.

### Builder Agent

Converts project inputs into technical execution.

Responsibilities:

- Architecture design
- ADR drafting
- Implementation planning
- Technical decomposition
- Code/design review support
- Delivery-risk analysis

### Reviewer Agent

Acts as a critical architecture reviewer.

Responsibilities:

- Challenge assumptions
- Identify missing alternatives
- Review scalability, security, reliability, and operational risks
- Push Builder outputs to a higher quality bar

### Explorer Agent

Looks beyond current delivery.

Responsibilities:

- Track emerging technologies
- Identify PoC opportunities
- Compare industry patterns
- Maintain an innovation backlog
- Feed future-facing ideas into Strategist and Builder

### Strategist Agent

Converts technical work into leadership-ready communication.

Responsibilities:

- Executive summaries
- Vision narratives
- Roadmap framing
- Decision memos
- Promotion evidence
- Stakeholder communication

### Navigator Agent

Runs separately from work-specific context.

Responsibilities:

- Career direction
- Role selection
- Skill-gap analysis
- Interview preparation
- Long-term positioning
- Sanitized achievement tracking

## Communication Model

Agents communicate through explicit handoff templates, not raw uncontrolled context sharing.

Typical flow:

```text
Project Agent
    ↓
Human-auditable task packet
    ↓
Builder Agent
    ↓
Reviewer Agent
    ↓
Builder revision
    ↓
Strategist Agent
    ↓
Human decision/action
```

Explorer and Strategist remain in sync so that executive communication includes not only delivery status, but also future vision.

Navigator receives only sanitized weekly or monthly summaries.

## Repository Structure

The `agents/` directory contains concrete or sample agent instances. The `templates/` directory contains copyable agent definitions and artifacts used when creating a project workspace. Shared schemas, taxonomies, and reusable cross-agent definitions belong in `templates/common/`. Root-level calibration files capture professional character and architecture philosophy. The `profiles/` directory contains optional personal overlays for a specific architect.

```text
architect-agentic-os/
  README.md
  architect-personality.md
  architecture-philosophy.md

  agents/
    sample-project-agent/
    sample-builder-agent/
    explorer/
    reviewer/
    strategist/
    navigator/

  templates/
    project-agent/
    builder-agent/
    explorer/
    reviewer/
    strategist/
    navigator/
    common/
    task-packets/
    handoffs/
    reviews/
    summaries/
    adr/
    planning/
    testing/
    exec-communication/

  profiles/
    krishna/
      builder-operating-rules.md
      project-operating-rules.md
      explorer-opportunity-scoring.md
      reviewer-review-taxonomy.md
      strategist-narrative-frameworks.md

  projects/
    sample-project/
      project-brief.md
      current-state.md
      decision-log.md
      risks.md
      task-packets/

  workflows/
    daily-checkin.md
    weekly-review.md
    monthly-strategy-review.md
    quarterly-career-review.md
```

## Safety and Confidentiality

This repository is intended to be public-safe.

Do not commit:

- Company source code
- Internal documents
- Customer information
- Private Slack/email content
- Roadmaps or confidential strategy
- Credentials, tokens, API keys, or secrets

Use this repository for reusable templates, agent charters, workflows, and professional operating principles.

Project-specific confidential work should remain in private local workspaces or company-approved repositories.

## Getting Started

1. Create the permanent agent charters.
2. Create the task packet template.
3. Create one sample project workspace.
4. Run one Project Agent for one active project.
5. Review its task packets manually.
6. Feed approved packets to the Builder Agent.
7. Run Reviewer review.
8. Use Strategist to convert the output into leadership-ready communication.
9. Send only sanitized weekly summaries to Navigator.

## Design Philosophy

This system is built around five principles:

1. **Clear role separation**  
   Each agent should have a narrow, durable purpose.

2. **Context hygiene**  
   Project-specific context should not pollute reusable professional memory.

3. **Human auditability**  
   Important agent outputs should pass through reviewable task packets or handoff documents.

4. **Portable character**  
   Professional principles, checklists, and communication style should outlive any project or job.

5. **Career compounding**  
   The system should help produce better architecture, better communication, stronger influence, and long-term career growth.

## Status

This project is currently in early design.

Planned next steps:

- Agent charters
- Task packet templates
- Handoff templates
- Review checklists
- Memory templates
- Daily and weekly operating workflows
- Example project setup
