# Architecture Decision Records

One file per decision, named `NNNN-short-title.md` (e.g. `0001-thehive-cortex-over-misp-opencti-connectors.md`), numbered sequentially and never renumbered even if superseded.

## Template

```markdown
---
title:
doc_type: architecture
domain: cross-domain
owner:
status: draft        # draft | accepted | superseded
last_reviewed:
review_cadence_days: 365
related_docs: []      # link the ADR it supersedes, if any
agent_executable: false
sensitivity: internal
---

# {NNNN} — {Decision Title}

## Context
What situation forced this decision — constraints, requirements, options on the table.

## Decision
What was decided, stated plainly.

## Alternatives considered
What else was evaluated and why it was ruled out.

## Consequences
What this decision makes easier, what it makes harder, and what it locks in for later.
```
