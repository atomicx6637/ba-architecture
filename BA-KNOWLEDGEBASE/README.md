# Business Architecture Knowledgebase (Sample)
## How to navigate and use this set of artifacts

This folder is a sample, cross-linked BA knowledgebase for a vertically integrated utility. Use it as a starting point for structuring strategy-to-execution content and for demonstrating traceability across domains.

## Quick start
- Start with `1-FOUNDATION/ba-kb.md` (overall blueprint), `ba-principles.md`, and `ba-standards.md` to understand scope and conventions.
- Strategy: `2-STRATEGY/ent-strategic-plan.md`, `ent-strategic-objectives.md`, `ent-strategic-roadmaps.md`, and `ent-strategy-capability-mapping.md` define intent and its link to capabilities.
- Core models: `3-CAPABILITIES/ent-capabilities-l1-l2.md` and `4-VALUE-STREAMS/ent-value-streams-catalog.md` plus their mappings (`ent-capability-to-org-mapping.md`, `ent-value-stream-capability-mapping.md`).
- Execution: initiatives and dependencies in `9-INITIATIVES`, metrics in `11-METRICS`, and governance in `14-GOVERNANCE`.
- Views: curated consumables live in `12-ARCHITECTURE-VIEWS` and cross-domain indexes in `13-CROSS-DOMAIN-MAPPINGS`.

## Domain map (what lives where)
- `1-FOUNDATION`: charter, governance, glossary, standards.
- `2-STRATEGY`: strategic plan/themes/objectives, capability alignment, roadmaps.
- `3-CAPABILITIES`: capability model (L0–L3), definitions, assessments, org mapping.
- `4-VALUE-STREAMS`: value stream catalogs, pain points, performance, capability enables.
- `5-STAKEHOLDERS`: stakeholder catalog, value props, engagement plans, segment views.
- `6-PRODUCTS`: product catalog (regulated/non-regulated), lifecycle, metrics, mappings.
- `7-INFORMATION`: business information model, data quality and master data strategy, entity and flow examples, capability mapping.
- `8-ORGANIZATION`: operating model, structure, roles, RACI and capability alignment.
- `9-INITIATIVES`: portfolio, prioritization, dependencies, value realization, exemplar initiative sheets.
- `10-POLICIES`: corporate/regulatory policies, tariffs/terms, policy-capability links.
- `11-METRICS`: strategic, capability, value stream, and initiative metrics plus scorecards.
- `12-ARCHITECTURE-VIEWS`: executive, transformation, domain, and business-unit views.
- `13-CROSS-DOMAIN-MAPPINGS`: quick-link indexes across domains (strategy, capabilities, products, stakeholders, policies).
- `14-GOVERNANCE`: change/review cycles, quality and tool standards, comms.

## Traceability recipes (sample flows)
- Connect strategy to change: objectives (`2-STRATEGY`) → capabilities (`3-CAPABILITIES`) → initiatives and dependencies (`9-INITIATIVES`) → metrics (`11-METRICS`).
- Tie products to value: product catalog (`6-PRODUCTS`) → value streams (`4-VALUE-STREAMS`) → stakeholder value propositions (`5-STAKEHOLDERS`) → policy impacts (`10-POLICIES`).
- Land governance: apply lifecycle and review cadence (`14-GOVERNANCE/ba-review-cycles.md`) and quality standards (`ba-quality-standards.md`) to any new artifact.

## Working conventions
- `ent-*` files are canonical enterprise views; folders with scenario examples (e.g., `capability-model-l3-detailed/`, `initiatives/`) show sample instances.
- Keep document headers (version/date/scope) updated when you materially change content; use annual reviews in `14-GOVERNANCE/ba-review-cycles.md`.
- Prefer linking to canonical sources instead of duplicating content; use `13-CROSS-DOMAIN-MAPPINGS` as entry points when adding new mappings.
- When adding domain content, include: purpose, scope, audience, concerns, and document control to stay consistent with the existing pattern.
