# Current State Architecture View
## Quantum Energy - "As-Is" Business and Technology Landscape

**Document Version:** 1.0
**Date:** 2025-11-25
**Scope:** High-level conceptual overview of Quantum Energy's current business and technology architecture
**Target Audience:** ELT, Architects, Transformation Leads, Business Leaders
**Concerns Addressed:** Understanding the existing state, identifying pain points, establishing a baseline for transformation.
**Primary Domains Covered:** Capabilities, Value Streams, Information, Technology, Organization
**Key Source Artifacts:**
*   [Enterprise Capabilities - Level 1 and Level 2](../../3-CAPABILITIES/ent-capabilities-l1-l2.md)
*   [Enterprise Value Streams Catalog (ent-value-streams-catalog.md)](../../4-VALUE-STREAMS/ent-value-streams-catalog.md)
*   [Enterprise Business Information Model - Conceptual (ent-business-information-model.md)](../../7-INFORMATION/ent-business-information-model.md)
*   [Current State Capability Maturity Assessment](../../3-CAPABILITIES/capability-assessments/capability-maturity-current.md)
*   [Value Stream Pain Points](../../4-VALUE-STREAMS/value-stream-pain-points.md)

---

## Executive Summary

This document presents a conceptual "As-Is" view of Quantum Energy's current business and technology architecture. It highlights key organizational components, capabilities, value streams, information domains, and technology systems as they exist today. The primary purpose of this view is to provide a common understanding of our current operating environment, identify existing challenges and pain points, and establish a baseline against which our strategic transformation efforts can be measured. This includes acknowledging the current state of both regulated utility operations and nascent non-regulated ventures.

---

## 1. Introduction

Understanding the current state is the first critical step in any transformation journey. This view captures the essence of how Quantum Energy currently operates, highlighting both functional strengths and areas ripe for improvement.

---

## 2. High-Level Current State Architecture Diagram (Conceptual)

```mermaid
C4Context
    title Quantum Energy Current State Architecture (Conceptual)

    Person(customer, "Customer", "Residential, Commercial, Industrial, Non-Regulated (EV, Smart Home, DG)")
    Person(regulator, "Regulator", "ESPUC, FERC, PHMSA, NERC")
    Person(employee, "Employee", "Regulated Ops, AES, Shared Services")

    System(ami_system, "AMI & MDMS", "Legacy AMI infrastructure for Electric/Gas meters, MDMS for data storage (limited real-time)")
    System(scada_gas, "SCADA/GMS", "Real-time control for Gas Distribution & Transmission (isolated)")
    System(scada_elec, "SCADA/EMS", "Real-time control for Electric T&D (some older components, limited DER visibility)")
    System(cis_billing, "CIS / Billing", "Core regulated Customer Info & Billing system (monolithic, limited self-service)")
    System(oms, "OMS", "Outage Management System (basic fault location, reactive customer communication)")
    System(ams_erp, "AMS / ERP", "Asset Management System (disparate instances, limited predictive capability) & Core Financials/HR/Procurement (on-prem, some manual processes)")
    System(aes_platform, "AES Product Platforms", "Cloud-based platforms for Smart Home, EV Charging, DG (early stage, some siloed data, nascent integrations)")
    System(crm_legacy, "Legacy CRM", "Separate, basic CRM systems for regulated service & non-regulated leads (fragmented customer view)")

    Boundary(regulated_ops, "Regulated Operations") {
        Rel(scada_gas, "Operates", customer, "Gas Service")
        Rel(scada_elec, "Operates", customer, "Electric Service")
        Rel(ami_system, "Feeds data to", cis_billing, "for billing")
        Rel(scada_elec, "Feeds data to", oms, "for outage detection")
        Rel(ams_erp, "Manages Assets for", scada_elec, "and", scada_gas)
    }

    Boundary(non_regulated_aes, "Non-Regulated AES Business Unit") {
        Rel(aes_platform, "Delivers Solutions to", customer, "Non-Regulated Offerings")
        Rel(aes_platform, "Collects data from", customer, "Smart Devices")
    }

    Boundary(enterprise_shared_services, "Enterprise Shared Services") {
        Rel(cis_billing, "Interacts with", crm_legacy)
        Rel(crm_legacy, "Manages interactions with", customer)
        Rel(ams_erp, "Supports", regulated_ops)
        Rel(ams_erp, "Supports", non_regulated_aes)
    }

    Rel(customer, "Receives Bills From", cis_billing)
    Rel(customer, "Reports Outages To", oms)
    Rel(customer, "Interacts with (Regulated)", crm_legacy)
    Rel(customer, "Interacts with (Non-Regulated)", aes_platform)
    Rel(employee, "Uses", ams_erp)
    Rel(employee, "Uses", cis_billing)
    Rel(employee, "Uses", scada_elec)
    Rel(employee, "Uses", aes_platform)

    Rel(regulator, "Oversight of", regulated_ops)
    Rel(cis_billing, "Provides Data for", regulator)
```

---

## 3. Key Observations & Pain Points

### 3.1. Organizational & Process Challenges

*   **Siloed Operations:** Clear division between Regulated Operations and AES, but limited formal collaboration mechanisms in operational planning or customer experience design.
*   **Manual Handoffs:** Significant manual effort in processes crossing functional or system boundaries, leading to inefficiencies and errors (e.g., data transfer for regulatory reporting, customer issue resolution).
*   **Talent Gaps:** Shortages in highly specialized digital skills (e.g., data scientists, cloud architects) and agile product development expertise.
*   **Change Management Fatigue:** Employees are often resistant to new technologies and process changes due to past experiences.

### 3.2. Capability Maturity & Gaps (As-Is)

*   **Regulated Strengths:** Strong core capabilities in Electric System Balancing & Dispatch (Level 4), Leak Detection & Pipeline Safety (Level 3) driven by regulatory mandates and decades of operational experience.
*   **Non-Regulated Nascent:** Non-Regulated Product Development and Customer Acquisition & Conversion (Level 2) are still nascent, lacking standardized processes and full market penetration.
*   **Enterprise Deficiencies:** Digital Customer Experience and Customer Insights & Analytics (both Level 2) are underdeveloped, resulting in fragmented customer journeys.
*(Refer to `../../3-CAPABILITIES/capability-assessments/capability-maturity-current.md` for details)*

### 3.3. Information & Data Challenges

*   **Fragmented Data:** Customer information resides in multiple, disconnected systems (CIS, CRM, AES platforms), preventing a unified customer view.
*   **Limited Real-Time Insights:** Operational data from SCADA/GMS is often isolated, hindering comprehensive real-time grid and operational analytics. AMI data is underutilized.
*   **Data Quality Issues:** Inconsistent data definitions and quality across disparate systems, impacting reporting and decision-making.
*   **Privacy Concerns:** Management of customer data from non-regulated smart devices raises new privacy and consent challenges.

### 3.4. Technology & Systems Landscape

*   **Legacy Systems:** Core regulated systems (CIS, Billing, some AMS) are often monolithic, difficult to integrate, and expensive to maintain.
*   **OT/IT Convergence:** Gaps in integration and security between operational technology (SCADA/EMS) and traditional IT systems.
*   **Siloed Platforms:** Non-regulated AES products are often built on separate, cloud-based platforms, leading to potential integration challenges with core utility systems.
*   **Limited Digital Enablement:** Lack of modern digital tools for field crews and customer self-service.

---

## 4. Business Pain Points (Conceptual)

*   **Customer Frustration:** Fragmented digital experiences, inconsistent service, and lack of personalized offers.
*   **High O&M Costs:** Due to manual processes, reactive maintenance, and suboptimal asset utilization.
*   **Slow Time-to-Market:** For new non-regulated products due to undeveloped product development capabilities and integration challenges.
*   **Regulatory Scrutiny:** Increased pressure on reliability metrics, safety compliance, and cost recovery.
*   **Cybersecurity Vulnerability:** Expanding attack surface with grid modernization and digital transformation.
*   **Data Inefficiency:** Inability to leverage full value of AMI and operational data for insights.

*(Refer to `../../4-VALUE-STREAMS/value-stream-pain-points.md` for details on specific value stream pain points)*

---

## Document Control

**Author:** Quantum Energy Enterprise Architecture Team, Business Architecture Team
**Reviewers:** ELT, BA Steering Committee, IT Leadership
**Approval:** Chief Enterprise Architect / Head of Business Architecture
**Version History:**
- v1.0 (2025-11-25): Initial Current State Architecture View for Quantum Energy.

**Next Review:** Annually or as transformation progresses

---

**End of Document**
