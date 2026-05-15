# Inception Standard

Twelve fields across three sections. A field is `complete` when its value is
concrete (domain-referencing, not template text) and meets the completeness
rule below. `partial` is OK if some but not all conditions are met. `pending`
means nothing captured yet.

## Product Vision
- **product_vision** — 2-4 sentences: what problem, for whom, why it matters. Min 50 chars, references domain.
- **target_users** — named user segments with context + needs. At least 2 distinct segments.
- **key_capabilities** — the 3-5 things the product must enable. At least 3 listed.
- **success_metrics** — measurable outcomes with numeric targets. At least 2 with numbers.

## Technical Approach
- **technical_approach** — architectural style + primary language/framework + persistence. Names at least one of each.
- **architecture_constraints** — hard constraints (must / must-not). At least 1.
- **dependencies** — external systems / libraries with protocols. All named.
- **risk_areas** — technical risks with code implications. At least 1 with specific impact.

## Phases and Sizing
- **phase_breakdown** — delivery phases with goals + exit criteria. At least 2.
- **effort_estimates** — sizing per phase.
- **dependency_order** — what must precede what. At least 1 chain.
- **timeline** — dates or duration per phase.
