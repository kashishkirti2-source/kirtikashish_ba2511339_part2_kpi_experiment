## Task 1: Business Problem Statement

The company conducted an A/B experiment to evaluate a new onboarding and activation campaign. New users were divided into a Control group using the existing onboarding experience and a Treatment group using the new onboarding campaign.

The objective is to determine whether the new onboarding experience should be launched to all users. The primary business metric is **Paid Conversion Rate**, as increasing paid customers directly supports business growth and revenue.

The decision should not rely only on conversion improvement. Guardrail metrics such as refund rate, support ticket rate, engagement score, average days to convert, and revenue quality must also be evaluated to ensure the treatment provides sustainable business value without negatively affecting user experience or profitability.


# Task 9: Recommendation Memo

## Executive Summary

An A/B experiment was conducted to evaluate whether the treatment improves the product's primary business objective compared with the control group. The treatment achieved a higher paid conversion rate and the improvement was statistically significant (p-value = 0.001146). However, additional guardrail metrics were evaluated to ensure that the increase in conversions did not negatively affect user experience or business performance.

---

# North Star Metric

**Paid Conversion Rate**

This metric represents the percentage of users who convert to a paid customer and directly reflects business growth and revenue generation.

---

# KPI Tree Explanation

**North Star Metric:** Paid Conversion Rate

Supporting KPIs:

* Landing Page Visit Rate
* Trial Start Rate
* Onboarding Completion Rate
* Paid Conversion Rate

Guardrail Metrics:

* Refund Rate
* Support Ticket Rate
* Average Days to Convert
* Average Engagement Score
* Revenue Quality (Average Revenue per Converted User)

These KPIs help measure both business growth and customer experience.

---

# Experiment Result Summary

| Metric                     | Control | Treatment |
| -------------------------- | ------- | --------- |
| Paid Conversion Rate       | 3.17%   | 6.99%     |
| Landing Page Visit Rate    | 63.64%  | 72.59%    |
| Trial Start Rate           | 25.11%  | 29.09%    |
| Onboarding Completion Rate | 15.58%  | 21.26%    |
| Average Revenue per User   | 51.75   | 53.88     |

The treatment outperformed the control group across the primary funnel metrics.

---

# Hypothesis Test Interpretation

A Chi-Square Test of Independence was performed on the Paid Conversion Rate.

* Significance Level (α): 0.05
* P-value: 0.001146

Since the p-value is less than 0.05, the null hypothesis is rejected.

This indicates that the increase in paid conversion rate is statistically significant and is unlikely to have occurred due to random variation.

---

# Guardrail Analysis

### Refund Rate

* Control: 0.00%
* Treatment: 0.42%

Refunds increased slightly but remained at a very low level.

### Support Ticket Rate

* Control: 21.93%
* Treatment: 37.20%

Support requests increased considerably in the treatment group, indicating potential usability or onboarding issues.

### Average Days to Convert

* Control: 8.86 days
* Treatment: 6.40 days

Users converted faster in the treatment group, which is a positive outcome.

### Average Engagement Score

* Control: 57.05
* Treatment: 62.90

User engagement improved after the treatment.

### Revenue Quality

* Average Revenue per Converted User

  * Control: 1630.10
  * Treatment: 770.41

Although more users converted, the revenue generated per converted user declined significantly and should be investigated.

---

# Segment-Level Insight

### Region Analysis

The treatment generated stronger average revenue across several regions, with the most noticeable improvements observed in the East and West regions.

### Device Type Analysis

Mobile and Tablet users showed higher engagement scores under the treatment compared to the control.

### Traffic Source Analysis

Organic Search and Referral channels produced more paid conversions under the treatment, while Social traffic showed relatively smaller gains.

---

# Final Recommendation

**Recommendation: Continue Testing**

The treatment significantly improves the paid conversion rate and user engagement while reducing the average time to convert. However, the increase in support ticket rate and the decrease in average revenue per converted user suggest that there are important business risks that should be addressed before a full rollout.

A phased rollout or additional experimentation is recommended to identify the causes of these guardrail issues.

---

# Risks and Limitations

* Increased support ticket volume may increase operational costs.
* Lower revenue per converted user may affect long-term profitability.
* Refund rate should continue to be monitored after rollout.
* Results are based on a single experiment and should be validated with additional testing.

---

# Next Steps

1. Investigate the causes of increased support tickets.
2. Analyze why revenue per converted user declined.
3. Run a follow-up A/B test focusing on pricing and onboarding improvements.
4. Monitor guardrail metrics during a phased rollout.
5. Validate results using a larger sample size before a complete launch.

