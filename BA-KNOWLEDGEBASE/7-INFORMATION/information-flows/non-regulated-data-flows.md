# Non-Regulated Data Flows - Key Exchanges within Advanced Energy Solutions
## Quantum Energy - Information Movement for Non-Regulated Services

**Document Version:** 1.0
**Date:** 2025-11-25
**Scope:** Key information flows specific to Quantum Energy's non-regulated advanced energy solutions
**Framework Standards:** BIZBOK, IoT Data Models
**Related Documents:**
*   [Enterprise Business Information Model - Conceptual (ent-business-information-model.md)](../ent-business-information-model.md)
*   [Non-Regulated Customer Information - Entity Definition](../information-entities/non-regulated-customer-info.md)
*   [Smart Device Data - Entity Definition](../information-entities/smart-device-data.md)
*   [NCV-01: Smart Home Solution Delivery - Stages](../../4-VALUE-STREAMS/value-stream-stage-models/non-regulated-solution-delivery-value-streams/ncv-01-smart-home-installation-stages.md)
*   [NCV-04: Non-Regulated Energy Advisory & Consulting](../../4-VALUE-STREAMS/ent-value-streams-catalog.md#ncv-04-non-regulated-energy-advisory-consulting)

---

## Executive Summary

This document details key information flows specific to Quantum Energy's non-regulated advanced energy solutions (AES) business unit. These flows are critical for the functionality of our products (e.g., smart home, EV charging), personalized customer insights, efficient service delivery, and rapid product iteration. Understanding these data exchanges ensures market agility, customer value creation, and strict adherence to data privacy and security protocols for non-regulated offerings.

---

## 1. Introduction

Non-regulated data flows govern the movement of information that supports Quantum Energy's advanced energy products and services. These flows often involve high-volume, granular data from customer-sited devices, requiring robust data management, analytics, and privacy capabilities to unlock value while mitigating risks.

---

## 2. Key Non-Regulated Data Flows

### 2.1. Smart Home Telemetry & Control Flow

**Description:** The continuous, bidirectional flow of data between customer-sited smart home devices and the Quantum Energy Smart Home Platform, enabling remote monitoring and control.

*   **Source:** Connected Device (Smart Thermostat, Smart Plug, etc.)
*   **Destination:** Quantum Energy Smart Home Platform (via Information Technology & Digital Services L1 Capability), Non-Regulated Customer Profile (for preferences), Energy Consumption Data (for aggregated device data).
*   **Key Information Entities Involved:** Connected Device, Device Telemetry, Device Control Log, Smart Home Automation Rule, Non-Regulated Customer Profile.
*   **Flow Steps:**
    1.  **Device Telemetry Transmission:** Smart devices send sensor data (e.g., temperature, power consumption) to the Smart Home Platform.
    2.  **Platform Processing & Storage:** Platform processes and stores telemetry data (often in time-series databases).
    3.  **Customer App/Portal Display:** Data is visualized on customer's mobile app/web portal.
    4.  **Customer/Automation Command:** Customer (via app) or automated rules (Smart Home Automation Rule) send control commands to the platform.
    5.  **Platform to Device Command:** Platform transmits commands to the respective smart device.
    6.  **Device Status Update:** Device reports execution status back to the platform.
*   **Privacy Importance:** Explicit customer consent is critical for data collection and usage.
*   **Market Importance:** Enables personalized experiences, product functionality, and customer engagement.

### 2.2. EV Charging Data & Management Flow

**Description:** The flow of data between EV charging stations, the EV Charging Network Platform, and customer accounts, managing charging sessions and optimizing energy use.

*   **Source:** Connected Device (EV Charger)
*   **Destination:** Quantum Energy EV Charging Network Platform (via Information Technology & Digital Services L1 Capability), Non-Regulated Customer Profile (for billing/preferences), Energy Consumption Data (for charging consumption).
*   **Key Information Entities Involved:** Connected Device (EV Charger), Device Telemetry (Charging Session Data), Non-Regulated Customer Profile, Non-Regulated Product Subscription.
*   **Flow Steps:**
    1.  **Charger Status & Availability:** EV chargers report real-time status (available, in use, fault) to the Network Platform.
    2.  **Charging Session Initiation:** Customer (via app/RFID) initiates a charging session.
    3.  **Charge Data Recording:** Network Platform records session details (start/end time, energy delivered, cost).
    4.  **Billing Data Flow:** Session data flows to billing system (via Financial Management L1 Capability) for non-regulated invoicing.
    5.  **Smart Charging Optimization:** Platform (via System Operations & Grid Control L1 Capability) may send commands to optimize charging based on grid signals or customer preferences.
    6.  **Customer App Display:** Customer app displays charging progress and session history.
*   **Market Importance:** Ensures efficient operation of charging network, accurate billing, and enables grid integration.
*   **Regulatory Separation:** Costing and pricing of charging sessions are separate from regulated electric rates.

### 2.3. Non-Regulated Product Sales & Onboarding Flow

**Description:** The flow of information from initial customer interest to successful sale and onboarding for non-regulated products.

*   **Source:** Non-Regulated Sales & Marketing (12.1-12.6 L2 Capabilities), Customer Engagement & Service (10.1 Customer Contact & Interaction Management)
*   **Destination:** Non-Regulated Customer Profile, Non-Regulated Product Subscription, Financial Management (for billing), Procurement & Supply Chain Management (for installation).
*   **Key Information Entities Involved:** Non-Regulated Customer Profile, Non-Regulated Product, Sales Opportunity, Non-Regulated Product Subscription, Non-Regulated Service Request.
*   **Flow Steps:**
    1.  **Lead Generation:** Marketing campaigns generate leads (Non-Regulated Customer Profile).
    2.  **Sales Qualification:** Sales team qualifies leads and identifies product interest.
    3.  **Solution Design & Quote:** Product specialists design solution and generate quote.
    4.  **Contracting & Sale:** Customer signs non-regulated service agreement.
    5.  **Order Fulfillment:** Order triggers installation scheduling (NCV-01, NCV-02, NCV-03 Value Streams).
    6.  **Customer Onboarding:** New customer is onboarded to non-regulated platform/service.
*   **Growth Importance:** Drives new revenue streams and customer acquisition for non-regulated business.

### 2.4. DER Aggregation & Grid Services Flow (Non-Regulated Assets)

**Description:** Data flow enabling the aggregation and optimized dispatch of customer-sited, non-regulated Distributed Energy Resources (DERs) for grid services or market participation.

*   **Source:** Connected Device (Solar Inverter, Battery Storage Unit), Energy Consumption Data (Meter Readings)
*   **Destination:** Quantum Energy DERMS (via System Operations & Grid Control L1 Capability), Wholesale Market Operator (External C), Financial Management (for payments/credits to customers).
*   **Key Information Entities Involved:** Connected Device (DER), Device Telemetry (DER Output), Energy Consumption Data (Net Metering), Non-Regulated Product Subscription (Grid Services Participation Program).
*   **Flow Steps:**
    1.  **DER Data Ingestion:** Real-time data from participating DERs flows to Quantum Energy's DERMS.
    2.  **DERMS Optimization:** DERMS analyzes grid conditions and market signals, optimizing DER dispatch.
    3.  **Dispatch Commands:** DERMS sends dispatch commands to participating DERs (e.g., curtail solar, discharge battery).
    4.  **Market Bid Submission:** Aggregated DER capacity is bid into wholesale markets (SMV-03).
    5.  **Settlement & Payments:** Market settlement data is processed, triggering payments/credits to DER owners.
*   **Strategic Importance:** Enables grid stability, integrates renewables, and creates new revenue streams for non-regulated offerings.
*   **Regulatory Interface:** DERMS interfaces with regulated grid operations for dispatch and receives market signals.

---

## 3. Data Governance Considerations for Non-Regulated Flows

*   **Explicit Consent:** Absolutely critical for all data collection, usage, and sharing from customer-sited devices, including for aggregation purposes.
*   **Privacy by Design:** Incorporating privacy controls into the design of all non-regulated products and data platforms.
*   **Security for IoT:** Enhanced cybersecurity measures to protect a diverse and potentially vulnerable IoT device ecosystem.
*   **Market Conduct & Fairness:** Ensuring transparency and fair practices in competitive markets, especially when leveraging regulated utility data or infrastructure.
*   **Data Monetization Ethics:** Clear ethical guidelines for any data monetization strategies for non-regulated data.
*   **Interoperability:** Working towards open standards and APIs for device and platform integration to maximize choice and flexibility for customers.

---

## Document Control

**Author:** Quantum Energy Business Architecture Team
**Reviewers:** Data Governance Council, Advanced Energy Solutions BU, IT Security, Legal, BA Review Board
**Approval:** Chief Data Officer, Chief Digital & Innovation Officer
**Version History:**
- v1.0 (2025-11-25): Initial definition of Non-Regulated Data Flows.

**Next Review:** Annually or upon significant changes to non-regulated product offerings, device integrations, or data privacy regulations

---

**End of Document**
