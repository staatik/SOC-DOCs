---
domain: cross-domain
---

# Metrics & Reporting

Where the SOC's own performance is measured and communicated — distinct from `architecture/`, which is about the SOC's design.

## Contents

- **SOC-CMM scorecards** — versioned snapshots of maturity scoring over time, so trend is visible, not just current state.
- **KPI/dashboard definitions** — MTTD, MTTR, alert-to-close ratios, detection coverage against ATT&CK, false-positive rate. Define the calculation, not just the number, so it's reproducible.
- **Executive reporting templates** — cadence and format for leadership-facing reports (distinct from incident-specific comms in `comms-templates/`).
- **Agent performance metrics** — once agents are handling investigations, track their accuracy/escalation rate here too, since it's a direct input to how much `agent_executable: true` scope is safe to expand.
