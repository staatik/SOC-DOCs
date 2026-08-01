---
domain: cross-domain
---

# SOC Business Continuity

What the SOC does when its own tooling is the thing that's down — degraded-mode operations, not customer/company-wide DR (that lives elsewhere in the org's BC/DR program; this folder is scoped to keeping detection and response functioning without primary tooling).

## Contents

- **SIEM-down procedures** — fallback detection sources and manual log review steps if Sentinel is unavailable.
- **Case-management-down procedures** — how IR continues if TheHive/Cortex is unreachable (this directly affects the agent trigger path described in `domains/agentic-ops/`, so document the manual fallback explicitly).
- **Communication fallback** — if primary comms tooling is down during an incident affecting it.
