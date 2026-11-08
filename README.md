# claude-architecture-decision-records-skill

A Claude Code skill for creating, reviewing, indexing, and maintaining Architecture Decision Records (ADRs).

## Overview

Architecture Decision Records capture why a significant technical decision was made, what alternatives were considered, and what consequences the team accepted. This skill helps teams preserve decision context so future contributors can understand the system's evolution.

## When to Use It

Use this skill when:

- Selecting a major technology or platform.
- Defining system or service boundaries.
- Choosing an architectural pattern.
- Making a significant data or integration decision.
- Accepting a material security or reliability trade-off.
- Reviewing or revisiting a historical decision.
- Establishing an ADR process for a team.

Do not create an ADR for every small implementation detail or routine code change.

## Recommended ADR Structure

1. **Title:** Short, descriptive decision name.
2. **Status:** Proposed, accepted, deprecated, or superseded.
3. **Context:** Problem, constraints, and decision drivers.
4. **Decision:** The selected approach.
5. **Alternatives:** Options considered and why they were not selected.
6. **Consequences:** Benefits, costs, risks, and follow-up work.
7. **References:** Internal artifacts needed to understand the decision, when appropriate.

## Installation

```bash
git clone https://github.com/Brajesh31/claude-architecture-decision-records-skill.git ~/.claude/skills/architecture-decision-records
```

## Usage

Invoke the skill when documenting or reviewing an architectural decision:

```text
/architecture-decision-records
```

Provide the decision context, constraints, candidate options, stakeholders, and the desired status.

## Decision Workflow

1. Confirm that the issue is architecturally significant.
2. Gather relevant requirements and constraints.
3. Identify realistic alternatives.
4. Compare trade-offs using consistent criteria.
5. State the decision clearly.
6. Record expected consequences and risks.
7. Assign follow-up actions where needed.
8. Add the ADR to the project's decision index.
9. Update status when the decision changes.
10. Preserve historical records rather than silently rewriting accepted decisions.

## Repository Template

The repository includes:

- `docs/adr/README.md`: ADR index and management guidance.
- `docs/adr/template.md`: Reusable ADR template.

Use the template consistently and adapt it to the project's existing documentation conventions.

## ADR Lifecycle

| Status | Meaning |
|---|---|
| Proposed | Under discussion |
| Accepted | Decision approved |
| Deprecated | No longer recommended |
| Superseded | Replaced by a newer decision |

## Quality Checklist

- The context explains why a decision is needed.
- Alternatives are realistic.
- The decision is unambiguous.
- Consequences include costs and risks.
- Status reflects the current state.
- Related follow-up work is assigned.
- Historical decisions remain discoverable.

## Repository Contents

- `SKILL.md`: Main ADR workflow and guidance.
- `docs/adr/README.md`: Decision index and lifecycle notes.
- `docs/adr/template.md`: Reusable ADR template.
- `README.md`: Overview and usage.

## Practical Principle

An ADR should explain the reasoning, not merely announce the selected technology. If a future engineer cannot understand the trade-off from the record, it is incomplete.
