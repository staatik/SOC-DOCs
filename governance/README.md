---
domain: cross-domain
---

# Governance & Policy

The authority layer everything else operates inside. Defines what the SOC and its analysts (human and agent) can and cannot do, and under whose approval.

## Contents

- **Charter** — mandate, scope, and authority of the SOC function.
- **RACI** — who's accountable/responsible/consulted/informed across SOC functions, especially at the seams (e.g. who owns a finding once it's handed to IT for remediation).
- **Acceptable-use / tool authorization policies** — what actions (containment, account disable, network isolation) are pre-authorized vs. require sign-off.
- **Escalation authority** — who can invoke the IR plan, notify legal/PR, or engage external counsel.
- **Agent authorization policy** — the governance analog for `agentic-ops/`: what actions an agent is authorized to take autonomously vs. must hand to a human. This is the policy `agent_executable: true` runbooks are ultimately accountable to.

Use [`/_templates/TEMPLATE-policy.md`](../_templates/TEMPLATE-policy.md) for new docs here.
