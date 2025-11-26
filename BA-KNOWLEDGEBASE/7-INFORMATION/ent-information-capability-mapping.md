# Enterprise Information - Capability Mapping
## Quantum Energy - Linking Data to Business Functions

**Document Version:** 1.0
**Date:** 2025-11-25
**Scope:** Mapping Quantum Energy's key information entities to the business capabilities that consume or produce them
**Framework Standards:** BIZBOK, DAMA-DMBOK
**Related Documents:**
*   [Enterprise Business Information Model - Conceptual (ent-business-information-model.md)](./ent-business-information-model.md)
*   [Enterprise Capabilities - Level 1 and Level 2](../../3-CAPABILITIES/ent-capabilities-l1-l2.md)

---

## Executive Summary

This document provides a crucial mapping between Quantum Energy's key business information entities and the capabilities that consume or produce them. Understanding these relationships is fundamental for effective data governance, system design, data quality management, and ensuring that our data assets effectively support business operations across both regulated and non-regulated segments.

---

## 1. Introduction to Mapping Methodology

This mapping links key Information Entities (from `ent-business-information-model.md` and related entity definitions) to the Level 1 and Level 2 Capabilities (from `ent-capabilities-l1-l2.md`) that primarily interact with that information. Interactions are classified as:

*   **Producer (P):** The capability is primarily responsible for creating, generating, or collecting the information.
*   **Consumer (C):** The capability primarily uses or processes the information.
*   **Both (B):** The capability both produces and consumes the information.

The mapping highlights whether the information entity primarily relates to Regulated (Reg), Non-Regulated (NonReg), or Enterprise (Ent) activities, and similarly for the capabilities.

---

## 2. Customer Information Domain - Capability Mapping

| Information Entity | Primary Scope | Producing/Consuming Capabilities (L1/L2 Examples) | Type of Interaction | Scope (Cap) |
| :----------------- | :------------ | :------------------------------------------------ | :------------------ | :---------- |
| **Customer Account (Regulated)** | Reg | 10. Customer Engagement & Service | B | Ent |
| | | 10.2. Customer Account Management | P | Ent |
| | | 14.2. General Accounting & Reporting | P | Ent |
| | | 3. Regulatory & Government Affairs | C | Reg |
| **Customer Profile (Regulated)** | Reg | 10. Customer Engagement & Service | B | Ent |
| | | 10.2. Customer Account Management | P | Ent |
| | | 10.8. Customer Insights & Analytics | C | Ent |
| | | 3. Regulatory & Government Affairs | C | Reg |
| **Non-Regulated Customer Profile** | NonReg | 12. Non-Regulated Sales & Marketing | B | NonReg |
| | | 11. Non-Regulated Product Development | C | NonReg |
| | | 10. Customer Engagement & Service | B | Ent |
| **Non-Regulated Product Subscription** | NonReg | 12. Non-Regulated Sales & Marketing | P | NonReg |
| | | 11. Non-Regulated Product Development | P | NonReg |
| | | 10. Customer Engagement & Service | C | Ent |
| **Premise** | Ent | 8. Electric Distribution | P | Reg |
| | | 9. Gas Distribution | P | Reg |
| | | 10. Customer Engagement & Service | B | Ent |
| | | 13. System Operations & Grid Control | C | Ent |

---

## 3. Energy Consumption & Metering Data Domain - Capability Mapping

| Information Entity | Primary Scope | Producing/Consuming Capabilities (L1/L2 Examples) | Type of Interaction | Scope (Cap) |
| :----------------- | :------------ | :------------------------------------------------ | :------------------ | :---------- |
| **Meter Point** | Ent | 9. Metering and Measurement | B | Ent |
| | | 9.1. Metering Infrastructure Management | P | Ent |
| | | 8. Electric Distribution | B | Reg |
| | | 9. Gas Distribution | B | Reg |
| **Meter** | Ent | 9. Metering and Measurement | B | Ent |
| | | 9.1. Metering Infrastructure Management | P | Ent |
| | | 8. Electric Distribution | B | Reg |
| | | 9. Gas Distribution | B | Reg |
| **Meter Reading** | Ent | 9. Metering and Measurement | B | Ent |
| | | 9.2. Meter Data Collection & Management | P | Ent |
| | | 14.2. General Accounting & Reporting | C | Ent |
| | | 10.8. Customer Insights & Analytics | C | Ent |
| | | 13. System Operations & Grid Control | C | Ent |
| **Consumption Profile** | Ent | 10.8. Customer Insights & Analytics | P | Ent |
| | | 9. Metering and Measurement | B | Ent |
| | | 11. Non-Regulated Product Development | C | NonReg |

---

## 4. Asset & Infrastructure Information Domain - Capability Mapping

| Information Entity | Primary Scope | Producing/Consuming Capabilities (L1/L2 Examples) | Type of Interaction | Scope (Cap) |
| :----------------- | :------------ | :------------------------------------------------ | :------------------ | :---------- |
| **Asset (Regulated)** | Reg | Asset Management | B | Reg |
| | | 8. Electric Distribution | B | Reg |
| | | 9. Gas Distribution | B | Reg |
| | | 5. Energy Generation | B | Reg |
| | | 7. Energy Transmission | B | Reg |
| | | 13. System Operations & Grid Control | B | Ent |
| | | 17. Procurement & Supply Chain Management | C | Ent |
| **Asset (Non-Regulated)** | NonReg | 11. Non-Regulated Product Development | B | NonReg |
| | | 12. Non-Regulated Sales & Marketing | P | NonReg |
| | | 10. Customer Engagement & Service | B | Ent |
| | | Asset Management | C | Reg |

---

## 5. Operational Information Domain - Capability Mapping

| Information Entity | Primary Scope | Producing/Consuming Capabilities (L1/L2 Examples) | Type of Interaction | Scope (Cap) |
| :----------------- | :------------ | :------------------------------------------------ | :------------------ | :---------- |
| **Grid State** | Reg | 13. System Operations & Grid Control | B | Ent |
| | | 13.2. Real-Time System Monitoring & Analysis | P | Ent |
| | | 8. Electric Distribution | B | Reg |
| | | 7. Energy Transmission | B | Reg |
| | | 5. Energy Generation | C | Reg |
| **Pipeline State** | Reg | 13. System Operations & Grid Control | B | Ent |
| | | 13.4. Gas System Balancing & Pressure Control | P | Ent |
| | | 9. Gas Distribution | B | Reg |
| | | 6. Natural Gas Supply & Storage | B | Reg |
| **Outage Event** | Ent | 13. System Operations & Grid Control | P | Ent |
| | | 8. Electric Distribution | B | Reg |
| | | 9. Gas Distribution | B | Reg |
| | | 10. Customer Engagement & Service | B | Ent |
| **Work Order** | Ent | Asset Management (Work & Resource Management L2) | B | Reg |
| | | 8. Electric Distribution | B | Reg |
| | | 9. Gas Distribution | B | Reg |
| | | 10. Customer Engagement & Service | P | Ent |
| **DER Dispatch** | Ent | 13. System Operations & Grid Control | P | Ent |
| | | 13.7. DER Management System (DERMS) Operations | P | Ent |
| | | 11. Non-Regulated Product Development | C | NonReg |

---

## 6. Financial & Regulatory Information Domain - Capability Mapping

| Information Entity | Primary Scope | Producing/Consuming Capabilities (L1/L2 Examples) | Type of Interaction | Scope (Cap) |
| :----------------- | :------------ | :------------------------------------------------ | :------------------ | :---------- |
| **Financial Transaction** | Ent | 14. Financial Management | B | Ent |
| | | 14.2. General Accounting & Reporting | P | Ent |
| | | 10. Customer Engagement & Service | C | Ent |
| | | 17. Procurement & Supply Chain Management | P | Ent |
| **Tariff/Rate Schedule** | Reg | 3. Regulatory & Government Affairs | P | Reg |
| | | 14. Financial Management | C | Ent |
| | | 10. Customer Engagement & Service | C | Ent |
| **Regulatory Filing** | Reg | 3. Regulatory & Government Affairs | B | Reg |
| | | 18. Legal & Compliance | B | Ent |
| | | 14. Financial Management | C | Ent |
| **Cost Allocation** | Ent | 14. Financial Management | P | Ent |
| | | 14.5. Regulatory Accounting & Cost Allocation | P | Ent |
| | | 3. Regulatory & Government Affairs | C | Reg |

---

## 7. Product & Market Information Domain - Capability Mapping

| Information Entity | Primary Scope | Producing/Consuming Capabilities (L1/L2 Examples) | Type of Interaction | Scope (Cap) |
| :----------------- | :------------ | :------------------------------------------------ | :------------------ | :---------- |
| **Product Definition** | Ent | 11. Non-Regulated Product Development | P | NonReg |
| | | 2. Market Development & Competitive Intelligence | C | Ent |
| | | 10. Customer Engagement & Service | C | Ent |
| **Market Segment** | Ent | 2. Market Development & Competitive Intelligence | P | Ent |
| | | 10. Customer Engagement & Service | C | Ent |
| | | 12. Non-Regulated Sales & Marketing | C | NonReg |
| **Competitor Profile** | Ent | 2. Market Development & Competitive Intelligence | P | Ent |
| | | 12. Non-Regulated Sales & Marketing | C | NonReg |
| **Sales Opportunity** | NonReg | 12. Non-Regulated Sales & Marketing | B | NonReg |
| | | 10. Customer Engagement & Service | C | Ent |
| **Smart Device Data** | NonReg | 11. Non-Regulated Product Development | C | NonReg |
| | | 13. System Operations & Grid Control | C | Ent |
| | | 10. Customer Engagement & Service | C | Ent |

---

## Document Control

**Author:** Quantum Energy Business Architecture Team
**Reviewers:** Enterprise Architecture, Data Governance Council, IT Leadership, BA Review Board
**Approval:** Chief Data Officer, Chief Information Officer
**Version History:**
- v1.0 (2025-11-25): Initial Enterprise Information - Capability Mapping for Quantum Energy.

**Next Review:** Annually or upon significant changes to business capabilities or data architecture

---

**End of Document**
