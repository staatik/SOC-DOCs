# Frontmatter Schema

Every doc in this library — regardless of domain or tier — opens with this YAML frontmatter block. It's the layer that makes the library queryable by both humans and tools (search, dashboards, and any agent that reads this corpus at execution time).

```yaml
---
title:                     # human-readable doc title
doc_type:                  # governance | architecture | process | playbook | runbook | reference
domain:                    # threat-intel | detection-engineering | vulnerability-management |
                            # infrastructure-engineering | incident-response | dfir | iam-nhi |
                            # data-log-management | agentic-ops | tooling | cross-domain
owner:                     # role or name accountable for accuracy
status:                    # draft | active | deprecated
last_reviewed:              # YYYY-MM-DD
review_cadence_days:        # e.g. 90, 180 — drives a staleness report
applicable_tools: []        # e.g. [sentinel, wiz, sentinelone, thehive, cortex] — empty if tool-agnostic
related_docs: []            # relative paths to docs this one depends on or is invoked by
agent_executable: true|false # can an agent run this end-to-end without a judgment call?
sensitivity: internal|restricted # restricted = contains live detection logic / creds handling — gate access accordingly
---
```

## Field notes

- **`doc_type` vs `domain`** — `doc_type` is the tier (the "how granular"), `domain` is the pillar (the "what area"). A doc is always exactly one of each. This is what lets you filter the library either way: "show me every runbook" or "show me everything in detection-engineering."

- **`agent_executable`** — the field that matters most given the agent work in `agentic-ops/`. Set `true` only once a runbook has been validated as fully deterministic — no branching that requires analyst judgment. Playbooks are `false` by default; if a specific scenario inside a playbook is actually deterministic, split it out into its own runbook rather than flipping the playbook's flag. Don't set `true` speculatively — an agent may act on it directly.

- **`status: deprecated`** — don't delete deprecated docs. Keep them with this status and a `related_docs` pointer to the replacement; postmortems and audits need to reconstruct what procedure was live at a given time.

- **`sensitivity`** — most runbooks/playbooks default to `internal`. Mark `restricted` anything containing live detection logic, credential handling steps, or specifics that would help an adversary evade detection if leaked (this is the same instinct as not open-sourcing vendor-specific SOPs — see root README).

- **`review_cadence_days`** — pair this with `last_reviewed` to generate a staleness report (e.g. a script that flags any doc past due). Suggested defaults: runbooks 90 days (tools change fast), playbooks 180 days, governance/architecture 365 days.
