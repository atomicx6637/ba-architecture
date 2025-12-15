# Business Architecture Standards
## Quantum Energy

**Document Version:** 1.0
**Date:** 2025-11-25
**Scope:** Standards and conventions for Business Architecture artifacts at Quantum Energy

---

## Executive Summary

This document defines the standards and conventions for the creation, maintenance, and consumption of Business Architecture (BA) artifacts at Quantum Energy. Adherence to these standards ensures consistency, quality, and interoperability across the BA knowledgebase, facilitating effective communication and decision-making for both regulated utility operations and non-regulated advanced offerings. These standards are aligned with BIZBOK guidelines and tailored for Quantum Energy's integrated enterprise.

---

## 1. General Principles

*   **BIZBOK Alignment:** All BA artifacts will align with the principles and metamodel defined in the Business Architecture Body of Knowledge (BIZBOK® Guide).
*   **Clarity & Conciseness:** Artifacts should be clear, concise, and easy to understand for their target audience, avoiding unnecessary jargon.
*   **Consistency:** A consistent look, feel, and structure across all artifacts is paramount.
*   **Completeness & Accuracy:** Artifacts must accurately reflect the current state and intended future state of the business.
*   **Actionability:** Artifacts should provide practical insights that drive decision-making and support Quantum Energy's strategic objectives.
*   **Segment Distinction:** Explicitly delineate between regulated, non-regulated, and enterprise-wide elements where relevant using prefixes and clear contextual descriptions.

---

## 2. Artifact Naming Conventions

All BA artifacts will follow a consistent naming convention to enhance discoverability and understanding within the knowledgebase.

**General Pattern:** `[ScopePrefix]-[Domain]-[ArtifactType]-[Qualifier].md`

### 2.1. Scope Prefixes

Used to indicate the primary business segment or scope of the artifact:

*   **`ent-` (Enterprise):** Artifacts applicable to Quantum Energy as a whole, covering both regulated and non-regulated aspects (e.g., `ent-capabilities-l1-l2.md`).
*   **`reg-` (Regulated):** Artifacts specific to regulated utility operations (e.g., `reg-electric-distribution-capabilities-l3.md`).
*   **`nonreg-` (Non-Regulated):** Artifacts specific to non-regulated offerings and business units (e.g., `nonreg-smart-home-product-catalog.md`).
*   **`util-` (Utility Core):** Artifacts pertaining to the core, undifferentiated functions of a utility, which might be regulated but also serve as a foundation for non-regulated (less common, `reg-` or `ent-` preferred).

### 2.2. Domain

Refers to the primary BIZBOK domain the artifact belongs to:

*   `capabilities`
*   `value-streams`
*   `products`
*   `stakeholders`
*   `information`
*   `organization`
*   `strategies`
*   `initiatives`
*   `policies`
*   `metrics`
*   `architecture-views`
*   `cross-domain-mappings`
*   `governance`
*   `foundation` (for overarching documents like `ba-principles.md`)

### 2.3. Artifact Type

Describes the specific type of document or model:

*   `catalog`
*   `model`
*   `map`
*   `definition`
*   `assessment`
*   `roadmap`
*   `plan`
*   `structure`
*   `flow`
*   `report`
*   `list`
*   `raci`
*   `principles`
*   `governance`
*   `standards`
*   `glossary`

### 2.4. Qualifier (Optional)

Provides additional specificity (e.g., L1-L2, customer-facing, future-state).

*   `l1-l2`, `l3-detailed`
*   `current-state`, `future-state`
*   `customer-facing`, `operations`
*   `kpis`, `scorecards`

### 2.5. Examples

*   `ent-capabilities-l1-l2.md`
*   `reg-customer-acquisition-value-stream.md`
*   `nonreg-smart-home-product-catalog.md`
*   `ent-stakeholder-catalog.md`
*   `ent-information-model-conceptual.md`
*   `ent-strategic-roadmaps.md`
*   `reg-rate-case-policy.md`
*   `ent-metrics-balanced-scorecard.md`

---

## 3. Documentation Format & Structure

### 3.1. Markdown (.md)

*   All textual artifacts will be created and maintained in Markdown format.
*   Markdown is preferred for its simplicity, readability, version control friendliness, and ease of conversion to other formats (HTML, PDF).

### 3.2. Document Header

Each Markdown document will start with a standardized header block:

```markdown
# [Document Title]
## Quantum Energy

**Document Version:** [X.Y]
**Date:** [YYYY-MM-DD]
**Scope:** [Brief description of document scope]
**Framework Standards:** [e.g., BIZBOK, Strategy to Reality] (if applicable)

---
```

### 3.3. Headings

*   Use `#` for Level 1 headings, `##` for Level 2, `###` for Level 3, etc.
*   Headings should be descriptive and follow a logical hierarchy.

### 3.4. Lists

*   Use `*` or `-` for unordered lists.
*   Use `1.` for ordered lists.

### 3.5. Code Blocks / Diagrams

*   Use backticks (``````) for inline code/terminology.
*   Use fenced code blocks (```language) for larger code snippets or pseudo-code.
*   **Diagrams:** Where diagrams are necessary (e.g., value stream maps, capability heatmaps), they should be:
    *   Embedded as images (PNG, SVG preferred) generated from a consistent tool (e.g., Draw.io, Lucidchart).
    *   Stored in a dedicated `_assets` subdirectory within the relevant domain folder.
    *   Referenced with clear captions and explanations within the Markdown file.
    *   Consider using Mermaid syntax for simple, text-based diagrams that can be rendered directly in Markdown viewers.

### 3.6. Cross-Referencing

*   Internal links between Markdown files should use relative paths (e.g., `[ba-capabilities.md](../3-CAPABILITIES/ent-capabilities-l1-l2.md)`).
*   External references should be clearly cited with full URLs.

---

## 4. Modeling Standards

### 4.1. Capabilities

*   **Levels:** Capabilities will be modeled at Level 0 (Enterprise), Level 1 (Strategic), Level 2 (Tactical), and Level 3+ (Operational).
*   **Definition:** Each capability will have a clear, concise definition stating "what" it does, independent of "how" or "who".
*   **Attributes:** Key attributes for capabilities include: Strategic Importance, Current Maturity, Target Maturity, Owning Organization(s), Enabling Information, Systems.
*   **Heatmaps:** Use consistent color coding for heatmaps (e.g., red for low maturity/high strategic importance, green for high maturity/low strategic importance).

### 4.2. Value Streams

*   **Definition:** Each value stream will define a clear Triggering Stakeholder, Receiving Stakeholder, Value Proposition, Entry Criteria, and Exit Criteria.
*   **Stages:** Value streams will be decomposed into sequential stages.
*   **Enabling Capabilities:** Each stage will explicitly map to the L2/L3 capabilities that enable its execution.
*   **Swimlanes:** Where visual models are used, swimlanes may represent organizational units or roles involved at each stage.

### 4.3. Products

*   **Definition:** Each product will have a clear description, value proposition, target customer segments, and delivery model.
*   **Enabling Capabilities:** Explicitly link products to the L1/L2 capabilities required for their delivery.
*   **Regulated/Non-Regulated:** Clearly distinguish product type and the regulatory/market context.

---

## 5. Version Control and Change Management

*   **Version Control System:** All BA artifacts will be managed in a Git repository.
*   **Branching Strategy:** Use a standard branching strategy (e.g., `main` for published, `develop` for in-progress, feature branches for individual work).
*   **Commit Messages:** Commit messages should be clear, concise, and indicative of the changes made.
*   **Change Log:** Each document's header will include a version history.

---

## 6. Glossary

*   A central `ba-glossary.md` document will define key terms, acronyms, and concepts used throughout the knowledgebase.
*   Domain-specific terms may also be defined within relevant artifacts for immediate context.

---

## Document Control

**Author:** Quantum Energy Business Architecture Team
**Reviewers:** BA Review Board
**Approval:** Chief Enterprise Architect / Head of Business Architecture
**Version History:**
- v1.0 (2025-11-25): Initial draft of Business Architecture Standards for Quantum Energy.

**Next Review:** Annual or as tool/methodology changes occur

---

**End of Document**
