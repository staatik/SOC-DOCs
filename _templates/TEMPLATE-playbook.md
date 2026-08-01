---
title:
doc_type: playbook
domain:
owner:
status: draft
last_reviewed:
review_cadence_days: 180
applicable_tools: []
related_docs: []
agent_executable: false
sensitivity: internal
---

# {Playbook Title}

## Scenario

What situation this playbook covers, and how an analyst recognizes they're in it (vs. a related scenario covered by a different playbook).

## Decision tree

Describe the branching logic. Use a simple indented structure or a Mermaid flowchart — whichever is clearer for the number of branches.

```
1. Is {condition A}?
   - Yes → go to 2a
   - No  → go to 2b
2a. {judgment call} → invoke [runbook X]
2b. {judgment call} → invoke [runbook Y]
```

For each branch, link out to the runbook that executes it — the playbook makes the *call*, the runbook does the *work*.

## Severity / escalation thresholds

What observations bump this from "handle at analyst level" to "page on-call" to "invoke IR plan / notify leadership." Be concrete about thresholds, not just "if severe."

## Judgment notes

Anything that doesn't reduce to a clean decision tree — known false-positive patterns, context a human needs to weigh, historical false alarms worth knowing about.

## Related docs

- Runbooks invoked by this playbook:
- Process doc this playbook sits inside:
- Escalates to:
