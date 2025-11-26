# Regulated Data Flows - Key Exchanges within Utility Operations
## Quantum Energy - Information Movement for Regulated Services

**Document Version:** 1.0
**Date:** 2025-11-25
**Scope:** Key information flows specific to Quantum Energy's regulated utility operations
**Framework Standards:** BIZBOK, Utility Industry Data Models
**Related Documents:**
*   [Enterprise Business Information Model - Conceptual (ent-business-information-model.md)](../ent-business-information-model.md)
*   [Regulated Customer Information - Entity Definition](../information-entities/regulated-customer-info.md)
*   [Energy Consumption Data - Entity Definition](../information-entities/energy-consumption-data.md)
*   [AOV-04: Electric Energy Delivery - Stages](../../4-VALUE-STREAMS/value-stream-stage-models/operations-value-streams/aov-04-electric-energy-delivery-stages.md)
*   [RCV-03: Regulated Billing & Payment](../../4-VALUE-STREAMS/ent-value-streams-catalog.md#rcv-03-regulated-billing-payment)

---

## Executive Summary

This document details key information flows specific to Quantum Energy's regulated utility operations. These flows are critical for the reliable and safe delivery of electricity and natural gas, accurate customer billing, efficient asset management, and strict adherence to regulatory requirements. Understanding these regulated data exchanges ensures operational integrity, compliance, and effective service provision.

---

## 1. Introduction

Regulated data flows govern the movement of information that directly supports Quantum Energy's core utility functions. These flows are often subject to stringent data quality, security, and audit requirements due to their importance for public safety, financial accuracy, and regulatory oversight.

---

## 2. Key Regulated Data Flows

### 2.1. Meter-to-Bill Flow

**Description:** The end-to-end process of collecting energy consumption data from regulated meters, validating it, and using it to generate customer bills.

*   **Source:** Metering and Measurement (9.2 Meter Data Collection & Management)
*   **Destination:** Financial Management (14.2 General Accounting & Reporting), Customer Engagement & Service (10.2 Customer Account Management)
*   **Key Information Entities Involved:** Meter Point, Meter, Meter Reading, Customer Account (Regulated), Financial Transaction.
*   **Flow Steps:**
    1.  **Meter Reading Collection:** AMI network automatically collects interval data from electric and gas meters.
    2.  **Meter Data Validation, Estimation, Editing (VEE):** Raw meter reads are processed to ensure accuracy, fill missing gaps, and identify anomalies.
    3.  **Meter Data Management System (MDMS) Storage:** Validated meter data is stored in the MDMS.
    4.  **Billing Determinant Calculation:** MDMS calculates billing determinants (e.g., peak demand, time-of-use consumption).
    5.  **Billing System Integration:** Billing determinants are transmitted to the Customer Information System (CIS) / Billing System.
    6.  **Bill Calculation:** CIS applies regulated tariffs and rates to calculate customer charges.
    7.  **Bill Generation & Delivery:** CIS generates and delivers the customer bill.
*   **Regulatory Importance:** Critical for accurate billing, regulatory compliance (e.g., rate application), and revenue assurance.

### 2.2. Grid Operational Data Flow

**Description:** The continuous flow of real-time and near real-time data from the electric grid infrastructure to the control center for monitoring, analysis, and control.

*   **Source:** Electric Distribution (8.1 Distribution System Operations & Control), Energy Transmission (7.1 Transmission System Operations), Energy Generation (5.1-5.5 Generation Operations)
*   **Destination:** System Operations & Grid Control (13.2 Real-Time System Monitoring & Analysis), Asset Management (12.5 Asset Performance Monitoring & Analytics)
*   **Key Information Entities Involved:** Asset, Operational Event, Grid State, Meter Reading (high-frequency).
*   **Flow Steps:**
    1.  **SCADA/EMS Data Acquisition:** RTUs (Remote Terminal Units) and IEDs (Intelligent Electronic Devices) transmit sensor data (voltage, current, frequency, breaker status) from substations, lines, and generation units to SCADA/EMS systems.
    2.  **Real-Time Visualization & Alarming:** Control room operators monitor the grid state through dashboards and receive alarms for abnormal conditions.
    3.  **Operational Data Storage:** Data historian stores real-time and historical operational data.
    4.  **Grid Control Commands:** Operators issue commands (e.g., open/close breakers, adjust generation) through SCADA/EMS.
    5.  **Data for Analytics:** Operational data flows to analytics platforms for grid optimization, predictive maintenance, and post-event analysis.
*   **Regulatory Importance:** Essential for NERC Reliability Standards compliance, public safety, and maintaining grid stability.

### 2.3. Gas Pipeline Operational Data Flow

**Description:** Real-time data flow from the natural gas pipeline network to the gas control center for pressure, flow, and integrity management.

*   **Source:** Gas Distribution (9.1 Distribution System Operations & Control), Gas Transmission & Storage (4.1 Pipeline Operations & Control, 4.3 Underground Storage Facility Operations)
*   **Destination:** System Operations & Grid Control (13.4 Gas System Balancing & Pressure Control)
*   **Key Information Entities Involved:** Asset (Pipeline, Regulator Station), Operational Event, Pipeline State.
*   **Flow Steps:**
    1.  **SCADA/GMS Data Acquisition:** Sensors along pipelines and at regulator/compressor stations transmit data (pressure, flow, temperature, valve status) to SCADA/GMS systems.
    2.  **Real-Time Monitoring & Control:** Gas control operators monitor pipeline conditions, manage pressures, and dispatch operational activities.
    3.  **Operational Data Storage:** Data historian stores real-time and historical pipeline data.
    4.  **Pressure Management Commands:** Operators issue commands to adjust pressure regulators or control valves.
*   **Regulatory Importance:** Critical for PHMSA pipeline safety compliance, public safety, and reliable gas delivery.

### 2.4. Outage Management Information Flow

**Description:** The flow of information triggered by an outage event, from detection to restoration and customer communication.

*   **Source:** Customer Engagement & Service (10.1 Customer Contact & Interaction Management), System Operations & Grid Control (13.2 Real-Time System Monitoring & Analysis)
*   **Destination:** Electric Distribution (8.6 Outage Management & Restoration), Customer Engagement & Service (10.6 Customer Communications & Notifications)
*   **Key Information Entities Involved:** Outage Event, Customer Account (Regulated), Premise, Asset (Distribution).
*   **Flow Steps:**
    1.  **Outage Detection:** AMI last-gasp, SCADA alarms, or customer calls initiate outage event.
    2.  **Outage Management System (OMS) Creation:** OMS creates and models the outage event, identifying affected customers.
    3.  **Customer Communication:** OMS/CIS triggers proactive customer notifications (email, SMS) and provides ETRs.
    4.  **Field Dispatch:** OMS dispatches work orders to field crews (Work & Outage Management L1 Capability).
    5.  **Restoration & Status Update:** Field crews update OMS on restoration progress.
    6.  **Customer Notification (Restored):** OMS/CIS notifies customers of power restoration.
*   **Regulatory Importance:** Directly impacts regulated reliability metrics (SAIDI/SAIFI) and customer satisfaction.

---

## 3. Data Governance Considerations for Regulated Flows

*   **Auditability:** All regulated data flows must be auditable to demonstrate compliance with regulatory requirements.
*   **Segregation:** Strict segregation of regulated data from non-regulated data where required by regulatory bodies, or to prevent cross-subsidization.
*   **Retention:** Adherence to defined data retention policies for all regulated operational, customer, and financial data.
*   **Security:** Enhanced cybersecurity for Critical Infrastructure Protection (CIP) as mandated by NERC, covering relevant data flows.
*   **Disaster Recovery:** Robust disaster recovery plans for all systems involved in regulated data flows to ensure business continuity.

---

## Document Control

**Author:** Quantum Energy Business Architecture Team
**Reviewers:** Data Governance Council, Grid Operations, Regulatory Affairs, Legal, BA Review Board
**Approval:** Chief Data Officer, Chief Operations Officer
**Version History:**
- v1.0 (2025-11-25): Initial definition of Regulated Data Flows.

**Next Review:** Annually or upon significant changes to regulated operations or regulatory requirements

---

**End of Document**
