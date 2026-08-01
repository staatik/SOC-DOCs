---
domain: threat-intel
---

# Threat Intel

Adversary tracking and TTP/IOC ingestion (OpenCTI/MISP). Owns *what threats exist* — the intel-to-detection handoff lives here, not the rule mechanics.

## Structure

| Folder | Contents |
|---|---|
| [`process/`](./process/) | Cross-functional workflow docs |
| [`playbooks/`](./playbooks/) | Judgment-based response guides (PRO) |
| [`runbooks/`](./runbooks/) | Deterministic step-by-step SOPs |
| [`reference/`](./reference/) | Lookup content cited by the above |

New docs in this domain should use the templates in [`/_templates/`](../../_templates/) and follow the frontmatter schema in [`/_templates/FRONTMATTER-SCHEMA.md`](../../_templates/FRONTMATTER-SCHEMA.md).
