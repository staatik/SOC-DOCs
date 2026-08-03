---
domain: cross-domain
---

# Architecture & Strategy

This is where "SOC Architecture" from the original ask lives — the holistic view of the SOC as a system, not any one domain's internals.

## Contents

- **SOC-CMM assessment** — the maturity scoring artifact and its history over time (link to the `soc-maturity` project output).
- **Service map** — tool-agnostic map of security services by category (SIEM, EDR, CSPM, TIP, case management, orchestration) rather than by vendor product, so the map survives a tool swap.
- **[`adr/`](./adr/)** — Architecture Decision Records for the SOC's own tooling and design choices (e.g. "why TheHive+Cortex over MISP/OpenCTI connectors," "why Agent Zero over a custom framework").
- **[`diagrams/build-sequence.mmd`](./diagrams/build-sequence.mmd)** — the dependency map: what documentation gets built before what, phased from foundation through the agentic-ops layer. Rendered PNG sits alongside it (`diagrams/build-sequence.png`); regenerate after editing the `.mmd` source rather than hand-editing the PNG.

Architecture docs are strategic and infrequently changed — they explain *why the SOC is shaped the way it is*, distinct from `governance/` (*what's authorized*) and the `domains/` process docs (*how work actually flows*).
