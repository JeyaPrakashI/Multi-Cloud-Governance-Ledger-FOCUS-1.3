# Multi-Cloud FOCUS 1.3 Governance Ledger ☁️💰

**Role Positioning:** AI FinOps Lead | Platform Architect  
**Salary Target:** $10,500 – $15,000+ Tier

## 📌 Executive Summary
This project demonstrates a unified cloud financial ecosystem that normalizes billing data from **AWS, Azure, and Snowflake** into a single source of truth using the **FOCUS 1.3 Standard**. It features an automated governance layer that triggers self-healing protocols (auto-shutdown) when budget thresholds are breached.

---

## 🛠️ Technical Architecture
* **Data Standard:** FOCUS 1.3 (FinOps Open Cost & Usage Specification).
* **Ingestion:** Power Query transformation of fragmented CSV/JSON billing exports.
* **Visualization:** Power BI Executive Dashboard (1600x900 Resolution).
* **Governance:** Azure Budget Alerts integrated with Logic App automation.

---

## 🚦 Governance & Automation Logic
The dashboard tracks a high-risk "Development Lab" with the following automated lifecycle:
1.  **Threshold Detection:** Azure Monitor identifies spend exceeding **$0.80** (80% of $1.00 budget).
2.  **Webhook Trigger:** An HTTP Webhook signal is sent to `Logic-App-Stop-VM`.
3.  **Self-Healing:** The Logic App deallocates all non-production VMs to halt spend.
4.  **Final State:** The dashboard captures the finalized cost of **$0.85**, validating the successful intervention.

---

## 📊 Business Impact
* **Visibility:** Consolidated a 75.78% spend concentration in Snowflake ($255.00) for executive review.
* **Efficiency:** Separated Production ($317.15) from Experimental ($19.35) spend to identify waste.
* **Risk Mitigation:** Eliminated 100% of "Runaway Lab Spend" through policy-based automation.

---

## 📁 Repository Structure
* `/Dashboard/`: .PBIT Template file for the 1600x900 canvas.
* `/Data/`: Mock FOCUS 1.3 normalized datasets for AWS, Azure, and Snowflake.
* `/Automation/`: Logic App workflow definitions (JSON).
