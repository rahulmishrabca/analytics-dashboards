# Analytics Dashboards & Reports

Monthly business reporting and funnel health analysis for **BNPL / Postpaid lending** products.  
All data is anonymized and uses representative figures.

---

## 📁 Reports

### 1. `01_april_funnel_health_report.md`
**Monthly Postpaid Funnel Health Dashboard — April 2026**

A full monthly business review covering lead volume, conversion rates, rejection rates, and stage-wise funnel drop-off across three product variants (Delite, Lite, Mini). Includes anomaly flags, executive summary, and actionable recommendations for product and risk teams.

Key sections: Executive summary table, variant-level breakdown, stage funnel analysis, anomaly log, recommendations

---

## 💡 What These Reports Demonstrate

- **End-to-end reporting** — from raw SQL output to stakeholder-ready summary
- **Multi-dimensional analysis** — by product variant, funnel stage, and time period
- **Anomaly identification** — surfacing issues within regular reporting cycles
- **Business recommendations** — translating numbers into decisions for product, risk, and finance teams
- **Finance-ready data validation** — ensuring accuracy before handoff

---

## 📐 Report Structure (Standard Template)

Every monthly report follows this structure:

1. Executive Summary — top-line KPIs with MoM change
2. Product Variant Breakdown — Delite / Lite / Mini performance
3. Funnel Stage Analysis — where leads drop and by how much
4. Anomalies Flagged — issues detected during the month
5. Recommendations — prioritized actions for stakeholder teams

---

## 🛠️ Tools Used

- Trino SQL — data extraction from Hive tables
- PySpark — large dataset aggregations on EMR
- Excel — final report formatting and charts
- Slack — stakeholder communication and anomaly alerts

---

## 📌 Context

Reports cover the **Postpaid BNPL lending** domain. Figures are anonymized.  
Linked investigation write-ups are in the [`data-storytelling`](https://github.com/rahulmishrabca/data-storytelling) repo.
