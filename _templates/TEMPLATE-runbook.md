---
title:
doc_type: runbook
domain:
owner:
status: draft
last_reviewed:
review_cadence_days: 90
applicable_tools: []
related_docs: []
agent_executable: false
sensitivity: internal
---

# {Runbook Title}

## Trigger

What alert, ticket, or condition starts this runbook. Be specific — the exact alert name, source, or queue.

## Prerequisites

- Access/permissions needed
- Tools that must be open
- Preceding runbooks or checks that must already be complete

## Steps

1. **{Action}** — exact click path, query, or command. Include screenshots or exact KQL/SPL/CLI where relevant.
2. **{Action}** —
3. **{Action}** —

> Keep each step atomic and unambiguous — this is the tier where "use judgment" should never appear. If a step branches, that branch either belongs in a linked playbook, or should be expressed here as an explicit if/then with no ambiguity left.

## Expected outcome

What "done" looks like — the artifact, ticket state, or system state this runbook should produce.

## Escalation

If the outcome doesn't match, or a step fails: who/what queue to escalate to, and what context to hand off.

## Related docs

- Process doc this runbook is invoked from:
- Playbook this runbook supports (if any):
- Reference docs cited:
