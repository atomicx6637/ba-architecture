# Formal Architectural Review

## ARB-2025-017: Core Middleware Platform Upgrade

- **Project:** Core Middleware Platform Upgrade (DEM-00174)
- **Lead Architect:** Frank Lee
- **Review Date:** October 15, 2025

### 1. Overview
This review assesses the architectural impact of upgrading the MessageBus platform from v3.1 to v4.5. This platform is a critical Tier-1 component that facilitates data exchange between several enterprise systems.

### 2. Current State Architecture
- The MessageBus v3.1 platform is hosted on-premise on two physical servers (active/passive cluster).
- It uses legacy point-to-point connections and proprietary adapters.
- **Connected Systems:**
    - **CRM (Salesforce):** Bi-directional sync of customer data.
    - **Billing System (Legacy):** One-way push of billing statements.
    - **ERP (SAP):** Bi-directional sync of financial data.
    - **Marketing Platform (Marketo):** One-way push of customer segments.

### 3. Proposed Future State Architecture
- MessageBus v4.5 will be deployed on a virtualized platform (VMware) for improved scalability and disaster recovery.
- It will be configured in an active/active cluster for high availability.
- All connections will be re-implemented using modern API standards (REST/JSON) where possible.
- The new platform will enforce OAuth 2.0 for all connections, significantly improving security.

### 4. Architectural Impacts & Dependencies
- **High Impact:** This project will require code changes, re-configuration, and extensive testing for **all four connected systems**.
- **Cross-Functional Dependency:** The project requires dedicated resources from the CRM, Billing, ERP, and Marketing application teams to work in concert during the testing and cutover phases.
- **Downtime:** A planned downtime window of 4-6 hours will be required for the final cutover.

### 5. Risks & Mitigation
- **Risk:** Integration failure post-migration.
    - **Mitigation:** A parallel test environment will be built to allow for full end-to-end testing before the production cutover.
- **Risk:** Performance degradation on connected applications.
    - **Mitigation:** Extensive load testing will be performed as part of the qualification phase.

### 6. Architectural Decision
The proposed future-state architecture is sound and aligns with EA principles of modernization, security, and high availability. The upgrade is a necessary and strategic step to reduce technical debt and mitigate business risk.

**Recommendation:** The Enterprise Architecture Board **approves** the proposed architecture. The Tier 2 classification is confirmed as appropriate due to the high degree of cross-portfolio dependency.
