# Monthly Postpaid Funnel Health Dashboard — April 2026

**Report Type:** Monthly Business Review  
**Product:** Postpaid BNPL  
**Audience:** Product, Risk, and Finance Teams  
**Prepared by:** Data & Business Analyst — Postpaid Team

---

## 📊 Executive Summary

| Metric | March 2026 | April 2026 | Change |
|---|---|---|---|
| Total Leads | 28,400 | 31,200 | +9.9% ↑ |
| Converted Accounts | 4,970 | 5,180 | +4.2% ↑ |
| Overall Conversion Rate | 17.5% | 16.6% | -0.9pp ↓ |
| Overall Rejection Rate | 38.2% | 41.5% | +3.3pp ↑ |
| Avg Time to Convert (days) | 3.2 | 3.8 | +0.6 days ↑ |

**Headline:** Lead volume grew 10% MoM but conversion rate dipped slightly — driven primarily by a temporary bureau pull failure in the first week of April (investigated separately). Underlying funnel health remains stable.

---

## 📦 Product Variant Breakdown

### Delite
| Metric | March | April | Change |
|---|---|---|---|
| Leads | 12,100 | 13,400 | +10.7% |
| Conversions | 2,230 | 2,280 | +2.2% |
| Conversion Rate | 18.4% | 17.0% | -1.4pp |
| Rejection Rate | 35.1% | 39.8% | +4.7pp |

### Lite
| Metric | March | April | Change |
|---|---|---|---|
| Leads | 9,800 | 10,600 | +8.2% |
| Conversions | 1,390 | 1,450 | +4.3% |
| Conversion Rate | 14.2% | 13.7% | -0.5pp |
| Rejection Rate | 40.3% | 43.1% | +2.8pp |

### Mini
| Metric | March | April | Change |
|---|---|---|---|
| Leads | 6,500 | 7,200 | +10.8% |
| Conversions | 1,350 | 1,450 | +7.4% |
| Conversion Rate | 20.8% | 20.1% | -0.7pp |
| Rejection Rate | 38.9% | 39.2% | +0.3pp |

---

## 🔍 Funnel Stage Analysis — April 2026

| Stage | Leads Entered | Leads Dropped | Drop-off % |
|---|---|---|---|
| Lead Created | 31,200 | — | — |
| Eligibility Check | 29,800 | 1,400 | 4.5% |
| Bureau Check | 24,600 | 5,200 | 17.4% |
| Offer Generation | 19,100 | 5,500 | 22.4% |
| User Acceptance | 8,400 | 10,700 | 56.0% |
| Account Activated | 5,180 | 3,220 | 38.3% |

**Key observation:** The largest absolute drop (10,700 leads) happens at the User Acceptance stage — leads receive an offer but do not accept. This is the biggest optimization opportunity for April.

---

## ⚠️ Anomalies Flagged This Month

1. **Bureau pull failure spike (April 3–9):** Failure rate hit 41% vs 4% baseline — traced to a backend config change. Resolved within 6 days. Full investigation in `data-storytelling` repo.
2. **Delite rejection rate increase:** Excluding the bureau failure week, Delite rejection rate still up 1.8pp — under review by Risk team.

---

## ✅ Recommendations

1. **User Acceptance drop-off:** Run A/B test on offer presentation UI — 56% drop suggests users may not understand the offer terms. Simplify the offer screen copy.
2. **Delite rejection review:** Risk team to audit bureau score thresholds for Delite — possible recalibration opportunity.
3. **Mini variant scale-up:** Highest conversion rate (20.1%) and steady rejection rate — good candidate for increased marketing spend.

---

## 🛠️ How This Report Was Built

- Stage funnel data pulled via Trino SQL on Hive tables
- Product variant breakdown from `lead_history_snapshot_v3` joined with `old_pp_accounts_data`
- Anomaly detection using 7-day rolling average rejection rate query
- Final tables assembled in Excel for stakeholder sharing
