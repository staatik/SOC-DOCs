---
domain: cross-domain
---

# Change Management

How a new or modified detection, playbook, or runbook gets reviewed and shipped — the meta-process that governs changes to everything else in this library.

## Contents

- **Review process** — who approves a new/changed runbook before `status: active`, and what review a change to an `agent_executable: true` doc specifically requires (this should be stricter than a human-only runbook, since a mistake here can execute unsupervised).
- **Versioning policy** — how doc history is tracked (git history is likely sufficient, but state that explicitly rather than leaving it implicit).
- **Detection rule change control** — specific to `domains/detection-engineering/`: staging/testing requirements before a rule goes live, and rollback procedure if a new rule causes alert flooding.
