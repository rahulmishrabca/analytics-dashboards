# Analytics Dashboards & Reports

> 🔗 **[▶ View Live Interactive Dashboard](https://rahulmishrabca.github.io/analytics-dashboards/)**

Interactive funnel analytics dashboard and monthly business reports for **BNPL / lending** products.
All data is anonymized and uses representative figures.

---

## 🚀 Live Dashboard

[![Dashboard Preview](https://img.shields.io/badge/Live_Dashboard-View_Now-2471A3?style=for-the-badge&logo=googlechrome&logoColor=white)](https://rahulmishrabca.github.io/analytics-dashboards/)

The interactive dashboard includes:

| Tab | What It Shows |
|---|---|
| 📅 **Monthly Funnel** | Stage-wise lead drop-off, MoM conversion trends, flow breakdown |
| 📆 **Daily View (30d)** | Day-level funnel performance, decile heatmap, daily anomaly flags |
| 🔴 **Stuck Cases** | Cases stuck at each stage by day — auto vs user action required |
| 🔬 **Rule Engine Analysis** | Rejection reason breakdown, rising trends, priority fix recommendations |

---

## 📁 Reports

### 1. `01_april_funnel_health_report.md`
**Monthly BNPL Funnel Health Dashboard — April 2026**

A full monthly business review covering lead volume, conversion rates, rejection rates, and stage-wise funnel drop-off. Includes anomaly flags, executive summary, and actionable recommendations for product and risk teams.

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
2. Product Variant Breakdown — performance across product lines
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

Reports cover the **BNPL lending** domain. All figures are anonymized and representative.
Linked investigation write-ups are in the [`data-storytelling`](https://github.com/rahulmishrabca/data-storytelling) repo.
