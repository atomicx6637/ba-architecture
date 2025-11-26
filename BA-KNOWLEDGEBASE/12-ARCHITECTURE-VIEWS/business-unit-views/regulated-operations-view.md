# Regulated Operations View
## Quantum Energy - Architecture Overview for Core Utility Services

**Document Version:** 1.0
**Date:** 2025-11-25
**Scope:** Architecture overview for Quantum Energy's Regulated Operations Division
**Target Audience:** COO, VPs Regulated Operations, Regulators, Program Managers
**Concerns Addressed:** Operational efficiency, service reliability, safety, regulatory compliance, asset management.
**Primary Domains Covered:** Capabilities, Value Streams, Information, Products
**Key Source Artifacts:**
*   [Enterprise Capabilities - Level 1 and Level 2](../../3-CAPABILITIES/ent-capabilities-l1-l2.md)
*   [Regulated Operations L3 Capabilities](../../3-CAPABILITIES/capability-model-l3-detailed/regulated-operations-l3.md)
*   [Enterprise Value Streams Catalog (ent-value-streams-catalog.md)](../../4-VALUE-STREAMS/ent-value-streams-catalog.md)
*   [Regulated Data Flows (regulated-data-flows.md)](../../7-INFORMATION/information-flows/regulated-data-flows.md)
*   [Regulated Tariffs and Rates (reg-tariffs-and-rates.md)](../../10-POLICIES/reg-tariffs-and-rates.md)

---

## Executive Summary

This document provides a high-level architectural view of Quantum Energy's Regulated Operations Division. It highlights the core capabilities, value streams, products, and information flows essential for the safe, reliable, and compliant delivery of electric and natural gas utility services. This view is critical for internal operational leaders, regulatory bodies, and program managers to understand the structure and functioning of our regulated business.

---

## 1. Introduction

The Regulated Operations Division is the backbone of Quantum Energy, responsible for delivering essential electric and natural gas services within our service territory. This view distills the complex interplay of assets, people, processes, and technology into a clear, concise architectural representation.

---

## 2. Key Regulated Products & Services

The following core products are the responsibility of Regulated Operations for their delivery and maintenance:
*   **ELEC-RES-001:** Residential Electric Service
*   **GAS-RES-001:** Residential Natural Gas Service
*   **ELEC-IND-001:** Industrial Electric Service
*   **GAS-IND-001:** Industrial Natural Gas Service
*   **DUAL-RES-001:** Dual-Fuel Residential Bundle
*(Refer to `ent-product-catalog.md` for full list and details)*

---

## 3. Core Regulated Capabilities

The following Level 1 Capabilities (and their L2 decompositions) are central to the Regulated Operations Division:

*   **5. Energy Generation:** (Reg)
    *   5.1. Conventional Generation Operations
    *   5.2. Renewable Generation Operations
    *   5.3. Generation Maintenance & Reliability
    *   5.4. Generation Scheduling & Dispatch
    *   5.5. Energy Storage Operations (Utility Scale)
    *   5.6. Fuel Procurement & Management
*   **6. Natural Gas Supply & Storage:** (Reg)
    *   6.1. Gas Commodity Procurement
    *   6.2. Interstate Pipeline & Storage Capacity Management
    *   6.3. Gas Supply Planning & Forecasting
    *   6.4. Gas Supply Operations & Balancing
    *   6.5. Supplier & Pipeline Relationship Management
*   **7. Energy Transmission:** (Reg)
    *   7.1. Transmission System Operations
    *   7.2. Transmission System Maintenance
    *   7.3. Transmission System Planning & Engineering
    *   7.4. Transmission Capacity & Congestion Management
    *   7.5. RTO/ISO Coordination & Compliance
*   **8. Electric Distribution:** (Reg)
    *   8.1. Distribution System Operations & Control
    *   8.2. Distribution System Maintenance & Repair
    *   8.3. Service Connections & Installations
    *   8.4. Distribution System Planning & Engineering
    *   8.5. Distribution Automation & Grid Modernization
    *   8.6. Outage Management & Restoration
    *   8.7. Vegetation Management
*   **9. Gas Distribution:** (Reg)
    *   9.1. Distribution System Operations & Control
    *   9.2. Distribution System Maintenance & Repair
    *   9.3. Service Connections & Installations
    *   9.4. Distribution System Planning & Engineering
    *   9.5. Leak Detection & Pipeline Safety
    *   9.6. Pressure Regulation & Monitoring

*(Refer to `ent-capabilities-l1-l2.md` for full definitions and L2 details)*
*(Refer to `regulated-operations-l3.md` for L3 decomposition examples)*

---

## 4. Key Regulated Value Streams

The following value streams represent the end-to-end processes for delivering core utility services and managing associated assets:

*   **AOV-01: Asset Lifecycle Management:** Ensures optimal performance and longevity of regulated infrastructure.
*   **AOV-02: Capital Project Delivery:** Manages construction and upgrades of regulated assets.
*   **AOV-03: Work & Outage Management:** Coordinates field work for regulated maintenance and emergencies.
*   **AOV-04: Electric Energy Delivery:** The core process for delivering electricity to customers.
*   **AOV-05: Natural Gas Delivery:** The core process for delivering natural gas to customers.
*   **AOV-06: System Reliability & Emergency Response:** Manages grid stability and emergency response for electric and gas.
*   **RCV-01: Regulated Customer Acquisition:** (Shared with Customer Affairs) Onboarding new utility customers.
*   **REV-01: Rate Case & Cost Recovery:** (Shared with Regulatory Affairs) Securing regulatory approval for rates.
*   **REV-02: Regulatory Compliance & Reporting:** (Shared with Regulatory Affairs) Ensuring adherence to all utility regulations.

*(Refer to `ent-value-streams-catalog.md` for full details)*

---

## 5. Critical Information & Data Flows

Information is the lifeblood of Regulated Operations. Key information entities and flows include:

*   **Asset Master Data:** Critical for asset management, maintenance, and regulatory reporting.
*   **Energy Consumption Data:** Collected from meters for billing and operational planning.
*   **Operational Data:** Real-time telemetry from SCADA/GMS, sensor data for grid/pipeline status.
*   **Outage Event Data:** Records of service interruptions for management and communication.
*   **Regulatory Filing Data:** Information compiled for compliance and rate cases.
*   **Key Data Flows:**
    *   **Grid Operational Data Flow:** (Real-time data from electric grid to control center).
    *   **Gas Pipeline Operational Data Flow:** (Real-time data from gas network to control center).
    *   **Outage Management Information Flow:** (Detection to restoration and customer communication).
    *   **Meter-to-Bill Flow:** (Meter data collection to billing).

*(Refer to `ent-business-information-model.md` and `regulated-data-flows.md` for more details)*

---

## 6. Regulatory & Organizational Context

*   **Regulatory Oversight:** Governed by federal (FERC, PHMSA, NERC) and state (ESPUC) regulations. Operations must strictly adhere to approved tariffs and safety standards.
*   **Organizational Structure:** Primarily managed by the Regulated Operations Division under the Chief Operating Officer (COO).
*   **Interfaces with AES:** Coordinates with Advanced Energy Solutions (AES) for DER interconnection, grid impact analysis of non-regulated solutions, and sometimes shares customer data (with consent) for broader energy management solutions.
*   **Shared Services:** Leverages Enterprise Services for IT, HR, Finance, Legal, and Procurement.

---

## 7. Strategic Focus & Initiatives

*   **Strategic Theme:** Grid Modernization & Resilience.
*   **Key Initiatives:**
    *   **DGPR-001:** Digital Grid Program (Enhancing capabilities 8.5, 13.7, 9.5).
    *   **OEF-001:** Operational Efficiency First Initiative (Optimizing AOV value streams).
    *   **NEST-001:** New Energy Solutions Transformation (Integrating utility-scale renewables).

*(Refer to `ent-initiative-portfolio.md` for full details)*

---

## Document Control

**Author:** Quantum Energy Business Architecture Team
**Reviewers:** COO, VPs Regulated Operations, Regulatory Affairs, BA Review Board
**Approval:** Chief Operations Officer (COO)
**Version History:**
- v1.0 (2025-11-25): Initial Regulated Operations View for Quantum Energy.

**Next Review:** Annually or upon significant operational/regulatory changes

---

**End of Document**
