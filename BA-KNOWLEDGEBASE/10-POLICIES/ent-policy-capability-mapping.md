# Enterprise Policy - Capability Mapping
## Quantum Energy - Governing Capabilities with Rules

**Document Version:** 1.0
**Date:** 2025-11-25
**Scope:** Mapping Quantum Energy's key policies and regulatory requirements to the business capabilities they govern or are governed by
**Framework Standards:** BIZBOK, Governance, Risk, and Compliance (GRC)
**Related Documents:**
*   [Enterprise Policy Catalog (ent-policy-catalog.md)](./ent-policy-catalog.md)
*   [Enterprise Capabilities - Level 1 and Level 2](../../3-CAPABILITIES/ent-capabilities-l1-l2.md)

---

## Executive Summary

This document provides a crucial mapping between Quantum Energy's key policies, regulations, and business rules and the underlying business capabilities that they govern, inform, or constrain. Understanding these relationships is fundamental for ensuring compliance, managing risks, driving operational consistency, and designing resilient processes across both regulated utility operations and non-regulated advanced energy solutions.

---

## 1. Introduction to Mapping Methodology

This mapping links key Policies/Rules (from `ent-policy-catalog.md` and related documents) to the Level 1 Capabilities (from `ent-capabilities-l1-l2.md`) that they directly impact. The relationship is indicated as either "Governs" or "Informs":

*   **Governs (G):** The policy/rule directly constrains, mandates, or dictates the execution of the capability. Non-compliance results in direct consequences.
*   **Informs (I):** The policy/rule provides guidance, principles, or context that shapes how the capability is executed.

The mapping highlights whether the policy/rule and capability primarily relate to Regulated (Reg), Non-Regulated (NonReg), or Enterprise (Ent) activities.

---

## 2. Regulatory Policies - Capability Mapping

| Policy/Regulation | Scope (Policy) | Impacted Capabilities (L1) | Type of Impact | Scope (Cap) |
| :---------------- | :------------- | :------------------------- | :------------- | :---------- |
| **Federal Power Act (FPA)** | Reg | 7. Energy Transmission | G | Reg |
| | | 5. Energy Generation | G | Reg |
| | | 13. System Operations & Grid Control | G | Ent |
| | | 3. Regulatory & Government Affairs | I | Reg |
| **Natural Gas Act (NGA)** | Reg | 6. Natural Gas Supply & Storage | G | Reg |
| | | 3. Regulatory & Government Affairs | I | Reg |
| **Pipeline Safety Act (PSA)** | Reg | 9. Gas Distribution | G | Reg |
| | | 6. Natural Gas Supply & Storage | G | Reg |
| | | 15. Human Capital Management (Safety Training) | G | Ent |
| | | 3. Regulatory & Government Affairs | I | Reg |
| **Clean Air Act (CAA)** | Reg | 5. Energy Generation | G | Reg |
| | | 3. Regulatory & Government Affairs | I | Reg |
| | | 17. Procurement & Supply Chain Management (Fuel) | I | Ent |
| **NERC Reliability Standards** | Reg | 7. Energy Transmission | G | Reg |
| | | 5. Energy Generation | G | Reg |
| | | 13. System Operations & Grid Control | G | Ent |
| | | 16. Information Technology & Digital Services (OT) | G | Ent |
| | | 16.4. Cybersecurity & Information Security (L2) | G | Ent |
| **Evergreen State Public Utilities Act (PUA)** | Reg | 8. Electric Distribution | G | Reg |
| | | 9. Gas Distribution | G | Reg |
| | | 14. Financial Management | G | Ent |
| | | 10. Customer Engagement & Service | G | Ent |
| | | 3. Regulatory & Government Affairs | I | Reg |
| **Evergreen State Clean Energy Transition Act (CETA)** | Reg | 5. Energy Generation | I | Reg |
| | | 8. Electric Distribution | I | Reg |
| | | 2. Market Development & Competitive Intelligence | I | Ent |
| | | 11. Non-Regulated Product Development | I | NonReg |
| **Evergreen State Customer Data Privacy Act (CDPA)** | Reg | 10. Customer Engagement & Service | G | Ent |
| | | 16. Information Technology & Digital Services | G | Ent |
| | | 18. Legal & Compliance | G | Ent |
| | | 11. Non-Regulated Product Development | G | NonReg |
| | | 12. Non-Regulated Sales & Marketing | G | NonReg |

---

## 3. Corporate Policies - Capability Mapping

| Policy/Regulation | Scope (Policy) | Impacted Capabilities (L1) | Type of Impact | Scope (Cap) |
| :---------------- | :------------- | :------------------------- | :------------- | :---------- |
| **Code of Business Conduct and Ethics** | Ent | All L1 Capabilities | I | Ent |
| | | 18. Legal & Compliance | G | Ent |
| | | 15. Human Capital Management | G | Ent |
| **Data Privacy and Protection Policy** | Ent | All L1 Capabilities (handling data) | G | Ent |
| | | 10. Customer Engagement & Service | G | Ent |
| | | 16. Information Technology & Digital Services | G | Ent |
| | | 11. Non-Regulated Product Development | G | NonReg |
| | | 18. Legal & Compliance | I | Ent |
| **Cybersecurity Policy** | Ent | All L1 Capabilities (using IT/OT) | G | Ent |
| | | 16. Information Technology & Digital Services | G | Ent |
| | | 13. System Operations & Grid Control | G | Ent |
| **EH&S Policy** | Ent | All Operational L1 Capabilities | G | Ent |
| | | 5. Energy Generation | G | Reg |
| | | 8. Electric Distribution | G | Reg |
| | | 9. Gas Distribution | G | Reg |
| | | 15. Human Capital Management | G | Ent |
| **Procurement and Supply Chain Policy** | Ent | 17. Procurement & Supply Chain Management | G | Ent |
| | | All L1 Capabilities (acquiring goods/services) | I | Ent |
| **Investment Governance Policy** | Ent | 1. Enterprise Strategy & Performance Management | G | Ent |
| | | 14. Financial Management | G | Ent |
| | | All L1 Capabilities (requesting investment) | I | Ent |

---

## 4. Key Observations & Implications

*   **Pervasive Impact of Regulations:** `Regulatory & Government Affairs` capabilities are crucial for managing compliance, but regulatory rules (Federal/State Acts, NERC, PHMSA) directly govern all core regulated operational capabilities (e.g., Energy Generation, Transmission, Distribution).
*   **Enterprise-wide Policy Reach:** Corporate policies (e.g., Code of Conduct, Cybersecurity, Data Privacy) apply across the entire organization, impacting nearly all capabilities in both regulated and non-regulated segments.
*   **Data Privacy & Non-Regulated Offerings:** The `Evergreen State Customer Data Privacy Act` and the `Data Privacy and Protection Policy` have a strong "Governs" relationship with non-regulated capabilities (e.g., Non-Regulated Product Development, Customer Engagement) due to the collection of granular customer and smart device data.
*   **Interdependence of Legal & Compliance:** The `Legal & Compliance` capability is a key enabler for ensuring all other capabilities operate within legal and ethical boundaries, often "Informing" or being "Governed By" relevant policies.
*   **Balancing Act:** This mapping underscores the constant balancing act Quantum Energy faces: ensuring strict compliance and safety in regulated operations, while fostering innovation and agility in non-regulated markets, all under the umbrella of enterprise-wide corporate governance.

---

## Document Control

**Author:** Quantum Energy Business Architecture Team
**Reviewers:** Legal, Regulatory Affairs, Compliance, BA Review Board
**Approval:** General Counsel, Chief Operations Officer, Chief Digital & Innovation Officer
**Version History:**
- v1.0 (2025-11-25): Initial Enterprise Policy - Capability Mapping for Quantum Energy.

**Next Review:** Annually or upon significant policy/regulatory changes

---

**End of Document**
