# Enterprise Value Stream - Capability Mapping
## Quantum Energy - Linking Value Delivery to Capabilities

**Document Version:** 1.0
**Date:** 2025-11-25
**Scope:** Mapping Quantum Energy's key value streams to enabling business capabilities
**Framework Standards:** BIZBOK
**Related Documents:**
*   [Enterprise Value Streams Catalog (ent-value-streams-catalog.md)](./ent-value-streams-catalog.md)
*   [Enterprise Capabilities - Level 1 and Level 2](../../3-CAPABILITIES/ent-capabilities-l1-l2.md)

---

## Executive Summary

This document provides a crucial mapping between Quantum Energy's key value streams and the underlying business capabilities that enable their execution. This mapping highlights how "what" we do (capabilities) enables "how" we deliver value (value streams) to our stakeholders, encompassing both regulated utility services and non-regulated advanced energy solutions. Understanding these relationships is fundamental for strategic planning, identifying capability gaps, optimizing operations, and fostering cross-functional collaboration.

---

## 1. Introduction to Mapping Methodology

This mapping links Quantum Energy's Value Streams (from `ent-value-streams-catalog.md`) to the Level 1 and Level 2 Capabilities (from `ent-capabilities-l1-l2.md`) that enable their stages. The relationship is indicated as either "Primary" or "Secondary":

*   **Primary (P):** The capability is fundamental and critical for the successful execution of the value stream or a significant portion of its stages. Significant reliance on this capability.
*   **Secondary (S):** The capability provides important support, data, or governance to the value stream, but is not central to its core execution.

The mapping distinguishes capabilities by their primary scope (Regulated, Non-Regulated, or Enterprise) to illustrate the integrated nature of Quantum Energy's business model.

---

## 2. Regulated Customer Value Streams - Capability Mapping

| Value Stream ID | Value Stream Name | Key Enabling Capabilities (L1/L2 Examples) | Relationship | Scope (Cap) |
| :-------------- | :---------------- | :----------------------------------------- | :----------- | :---------- |
| **RCV-01** | **Regulated Customer Acquisition** | Customer Engagement & Service (L1) | P | Ent |
| | | Customer Contact & Interaction Management (L2) | P | Ent |
| | | Electric Distribution (L1) | S | Reg |
| | | Gas Distribution (L1) | S | Reg |
| | | Metering and Measurement (L1) | S | Ent |
| | | Financial Management (L1) (Credit Assessment) | P | Ent |
| **RCV-02** | **Regulated Customer Service Delivery** | Customer Engagement & Service (L1) | P | Ent |
| | | Customer Inquiry & Complaint Resolution (L2) | P | Ent |
| | | System Operations & Grid Control (L1) | S | Ent |
| | | Electric Distribution (L1) | S | Reg |
| | | Gas Distribution (L1) | S | Reg |
| **RCV-03** | **Regulated Billing & Payment** | Financial Management (L1) (General Accounting & Reporting) | P | Ent |
| | | Customer Engagement & Service (L1) | P | Ent |
| | | Metering and Measurement (L1) | P | Ent |
| | | Legal & Compliance (L1) | S | Ent |
| **RCV-04** | **Regulated Customer Program Participation** | Customer Engagement & Service (L1) | P | Ent |
| | | Customer Communications & Notifications (L2) | P | Ent |
| | | Market Development & Competitive Intelligence (L1) (Program Design) | S | Ent |
| | | Financial Management (L1) (Incentive Processing) | S | Ent |
| **RCV-05** | **Regulated Service Disconnection & Reconnection** | Customer Engagement & Service (L1) | P | Ent |
| | | Financial Management (L1) (Collections) | P | Ent |
| | | Electric Distribution (L1) | P | Reg |
| | | Gas Distribution (L1) | P | Reg |
| | | Legal & Compliance (L1) | S | Ent |

---

## 3. Non-Regulated Customer Value Streams - Capability Mapping

| Value Stream ID | Value Stream Name | Key Enabling Capabilities (L1/L2 Examples) | Relationship | Scope (Cap) |
| :-------------- | :---------------- | :----------------------------------------- | :----------- | :---------- |
| **NCV-01** | **Smart Home Solution Delivery** | Non-Regulated Product Development (L1) | P | NonReg |
| | | Product Development & Engineering (L2) | P | NonReg |
| | | Non-Regulated Sales & Marketing (L1) | P | NonReg |
| | | Customer Engagement & Service (L1) | P | Ent |
| | | Procurement & Supply Chain Management (L1) (Materials & Inventory Mgt) | S | Ent |
| **NCV-02** | **EV Charging Solution Deployment** | Non-Regulated Product Development (L1) | P | NonReg |
| | | Product Development & Engineering (L2) | P | NonReg |
| | | Non-Regulated Sales & Marketing (L1) | P | NonReg |
| | | Electric Distribution (L1) (Interconnection) | S | Reg |
| | | Information Technology & Digital Services (L1) (Platform Management) | P | Ent |
| **NCV-03** | **Distributed Generation (DG) & Storage Solution Provision** | Non-Regulated Product Development (L1) | P | NonReg |
| | | Non-Regulated Sales & Marketing (L1) | P | NonReg |
| | | Electric Distribution (L1) (Interconnection) | S | Reg |
| | | Energy Generation (L1) (Renewable Operations expertise) | S | Reg |
| | | Procurement & Supply Chain Management (L1) | P | Ent |
| **NCV-04** | **Non-Regulated Energy Advisory & Consulting** | Non-Regulated Product Development (L1) | P | NonReg |
| | | Market Development & Competitive Intelligence (L1) | P | Ent |
| | | Customer Insights & Analytics (L2) | P | Ent |
| | | Non-Regulated Sales & Marketing (L1) | P | NonReg |

---

## 4. Asset and Operations Value Streams - Capability Mapping

| Value Stream ID | Value Stream Name | Key Enabling Capabilities (L1/L2 Examples) | Relationship | Scope (Cap) |
| :-------------- | :---------------- | :----------------------------------------- | :----------- | :---------- |
| **AOV-01** | **Asset Lifecycle Management** | Asset Management (L1) | P | Reg |
| | | Asset Lifecycle Planning (L2) | P | Reg |
| | | Energy Generation (L1) | S | Reg |
| | | Electric Distribution (L1) | S | Reg |
| | | Gas Distribution (L1) | S | Reg |
| | | Financial Management (L1) | S | Ent |
| **AOV-02** | **Capital Project Delivery** | Asset Management (L1) | P | Reg |
| | | Capital Planning & Project Execution (L2) | P | Reg |
| | | Procurement & Supply Chain Management (L1) | P | Ent |
| | | Legal & Compliance (L1) | S | Ent |
| | | Regulatory & Government Affairs (L1) | S | Reg |
| **AOV-03** | **Work & Outage Management** | Asset Management (L1) | P | Reg |
| | | Work & Resource Management (L2) | P | Reg |
| | | Electric Distribution (L1) | P | Reg |
| | | Gas Distribution (L1) | P | Reg |
| | | System Operations & Grid Control (L1) | P | Ent |
| | | Customer Engagement & Service (L1) | S | Ent |
| **AOV-04** | **Electric Energy Delivery** | Energy Generation (L1) | P | Reg |
| | | Energy Transmission (L1) | P | Reg |
| | | Electric Distribution (L1) | P | Reg |
| | | System Operations & Grid Control (L1) | P | Ent |
| | | Metering and Measurement (L1) | S | Ent |
| **AOV-05** | **Natural Gas Delivery** | Natural Gas Supply & Storage (L1) | P | Reg |
| | | Gas Distribution (L1) | P | Reg |
| | | System Operations & Grid Control (L1) | P | Ent |
| | | Metering and Measurement (L1) | S | Ent |
| **AOV-06** | **System Reliability & Emergency Response** | System Operations & Grid Control (L1) | P | Ent |
| | | Electric Distribution (L1) | P | Reg |
| | | Gas Distribution (L1) | P | Reg |
| | | Legal & Compliance (L1) (Cybersecurity) | P | Ent |
| | | Customer Engagement & Service (L1) | S | Ent |

---

## 5. Supply and Market Value Streams - Capability Mapping

| Value Stream ID | Value Stream Name | Key Enabling Capabilities (L1/L2 Examples) | Relationship | Scope (Cap) |
| :-------------- | :---------------- | :----------------------------------------- | :----------- | :---------- |
| **SMV-01** | **Electric Energy Supply & Trading** | Energy Generation (L1) | P | Reg |
| | | Energy Trading and Risk Management (L1) | P | Reg |
| | | System Operations & Grid Control (L1) | P | Ent |
| | | Financial Management (L1) | S | Ent |
| **SMV-02** | **Natural Gas Supply & Trading** | Natural Gas Supply & Storage (L1) | P | Reg |
| | | Energy Trading and Risk Management (L1) | P | Reg |
| | | System Operations & Grid Control (L1) | P | Ent |
| | | Financial Management (L1) | S | Ent |
| **SMV-03** | **Distributed Energy Resource (DER) Aggregation & Optimization** | System Operations & Grid Control (L1) (DERMS Operations) | P | Ent |
| | | Non-Regulated Product Development (L1) | P | NonReg |
| | | Customer Engagement & Service (L1) | S | Ent |
| | | Metering and Measurement (L1) | S | Ent |
| **SMV-04** | **Non-Regulated Energy Market Participation** | Non-Regulated Product Development (L1) | P | NonReg |
| | | Energy Trading and Risk Management (L1) | P | Reg |
| | | System Operations & Grid Control (L1) | P | Ent |
| | | Legal & Compliance (L1) | S | Ent |

---

## 6. Regulatory & External Affairs Value Streams - Capability Mapping

| Value Stream ID | Value Stream Name | Key Enabling Capabilities (L1/L2 Examples) | Relationship | Scope (Cap) |
| :-------------- | :---------------- | :----------------------------------------- | :----------- | :---------- |
| **REV-01** | **Rate Case & Cost Recovery** | Regulatory & Government Affairs (L1) | P | Reg |
| | | Rate Design & Cost Recovery (L2) | P | Reg |
| | | Financial Management (L1) | P | Ent |
| | | Legal & Compliance (L1) | P | Ent |
| | | Asset Management (L1) | S | Reg |
| **REV-02** | **Regulatory Compliance & Reporting** | Regulatory & Government Affairs (L1) | P | Reg |
| | | Regulatory Compliance & Reporting (L2) | P | Reg |
| | | Legal & Compliance (L1) | P | Ent |
| | | Information Technology & Digital Services (L1) | S | Ent |
| **REV-03** | **External Stakeholder Engagement** | Brand & Reputation Management (L1) | P | Ent |
| | | Regulatory & Government Affairs (L1) | P | Reg |
| | | Customer Engagement & Service (L1) | P | Ent |
| **REV-04** | **Environmental Stewardship & Compliance** | Regulatory & Government Affairs (L1) | P | Reg |
| | | Environmental Permitting & Compliance (L2) | P | Reg |
| | | Energy Generation (L1) | S | Reg |
| | | Legal & Compliance (L1) | S | Ent |

---

## 7. Enterprise Support Value Streams - Capability Mapping

| Value Stream ID | Value Stream Name | Key Enabling Capabilities (L1/L2 Examples) | Relationship | Scope (Cap) |
| :-------------- | :---------------- | :----------------------------------------- | :----------- | :---------- |
| **ESV-01** | **Enterprise Strategic Planning & Execution** | Enterprise Strategy & Performance Management (L1) | P | Ent |
| | | Market Development & Competitive Intelligence (L1) | P | Ent |
| | | Financial Management (L1) | S | Ent |
| | | Human Capital Management (L1) | S | Ent |
| **ESV-02** | **Talent Management** | Human Capital Management (L1) | P | Ent |
| | | Workforce Planning & Analytics (L2) | P | Ent |
| | | Learning & Development (L2) | P | Ent |
| **ESV-03** | **Financial Management & Reporting** | Financial Management (L1) | P | Ent |
| | | General Accounting & Reporting (L2) | P | Ent |
| | | Legal & Compliance (L1) | S | Ent |
| **ESV-04** | **Information Technology & Digital Service Delivery** | Information Technology & Digital Services (L1) | P | Ent |
| | | Cybersecurity & Information Security (L2) | P | Ent |
| | | Application Development & Management (L2) | P | Ent |
| **ESV-05** | **Enterprise Risk Management** | Enterprise Strategy & Performance Management (L1) | P | Ent |
| | | Enterprise Risk Management (L2) | P | Ent |
| | | Legal & Compliance (L1) | S | Ent |
| **ESV-06** | **Procurement & Supply Chain Management** | Procurement & Supply Chain Management (L1) | P | Ent |
| | | Strategic Sourcing & Category Management (L2) | P | Ent |
| | | Materials & Inventory Management (L2) | P | Ent |

---

## Document Control

**Author:** Quantum Energy Business Architecture Team
**Reviewers:** BA Review Board, Strategic Planning Office, Operations Leads
**Approval:** Chief Enterprise Architect / Head of Business Architecture
**Version History:**
- v1.0 (2025-11-25): Initial Enterprise Value Stream - Capability Mapping for Quantum Energy.

**Next Review:** Annually or upon significant changes to value streams or capabilities

---

**End of Document**
