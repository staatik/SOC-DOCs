---
domain: cross-domain
---

# Architecture & Strategy

This is where "SOC Architecture" from the original ask lives — the holistic view of the SOC as a system, not any one domain's internals.

## Contents

- **SOC-CMM assessment** — the maturity scoring artifact and its history over time (link to the `soc-maturity` project output).
- **Service map** — tool-agnostic map of security services by category (SIEM, EDR, CSPM, TIP, case management, orchestration) rather than by vendor product, so the map survives a tool swap.
- **[`adr/`](./adr/)** — Architecture Decision Records for the SOC's own tooling and design choices (e.g. "why TheHive+Cortex over MISP/OpenCTI connectors," "why Agent Zero over a custom framework").
- **Dependency map** — what depends on what (e.g. the agent-security layer's explicit dependency on the underlying SOC foundation being in place first).

Architecture docs are strategic and infrequently changed — they explain *why the SOC is shaped the way it is*, distinct from `governance/` (*what's authorized*) and the `domains/` process docs (*how work actually flows*).
