# Part 2: KPI Framework, Business Experiment Analysis & Decision Recommendation

## Business Context

A subscription-based digital product company launched a new onboarding and activation campaign to improve user conversion and early engagement. An A/B experiment was conducted where users were divided into a Control group (existing onboarding) and a Treatment group (new onboarding). The objective was to determine whether the new onboarding experience should be rolled out to all users based on business performance and statistical evidence.

---

# Dataset Description

The dataset contains user-level experiment data for both Control and Treatment groups. It includes user information, experiment group assignment, onboarding funnel metrics, revenue, engagement score, support tickets, refund requests, conversion information, and customer segments such as region, device type, traffic source, and plan type.

---

# North Star Metric Selected

**Paid Conversion Rate**

This metric was selected because it directly measures the percentage of users who become paying customers. Improving this metric supports business growth, customer acquisition, and revenue generation.

---

# KPI Tree Summary

The KPI Tree was created using Paid Conversion Rate as the North Star Metric.

Primary KPI Drivers:

* User Acquisition
* User Activation
* User Experience

Supporting Metrics:

* Landing Page Visit Rate
* Trial Start Rate
* Onboarding Completion Rate
* Engagement Score
* Average Revenue Per User

Guardrail Metrics:

* Refund Rate
* Support Ticket Rate
* Average Days to Convert
* Revenue Quality

---

# Experiment Analysis Approach

The experiment dataset was prepared before analysis by performing the following checks:

* Missing value validation
* Group count verification
* Duplicate user ID detection
* Binary value validation
* Revenue outlier review
* Segment distribution analysis

After data validation, experiment summary metrics were calculated for both Control and Treatment groups using Pivot Tables and Excel formulas.

A Chi-Square Test of Independence was performed to determine whether the improvement in Paid Conversion Rate was statistically significant.

---

# Hypothesis Test Summary

* Test Used: Chi-Square Test of Independence
* Primary Metric: Paid Conversion Rate
* Significance Level: 0.05
* P-value: 0.001146

Since the p-value is less than 0.05, the null hypothesis was rejected. The Treatment group showed a statistically significant improvement in Paid Conversion Rate compared with the Control group.

---

# Guardrail Metrics Considered

The following guardrail metrics were evaluated before making a recommendation:

* Refund Rate
* Support Ticket Rate
* Average Days to Convert
* Average Engagement Score
* Revenue Quality (Average Revenue per Converted User)

The analysis showed that although conversions increased, Support Ticket Rate also increased and Revenue Quality declined, indicating potential risks.

---

# Final Recommendation

**Recommendation: Continue Testing**

The Treatment significantly improved Paid Conversion Rate and user engagement while reducing the average time to convert.

However, higher Support Ticket Rates and lower Average Revenue per Converted User indicate business risks that should be investigated before a complete rollout.

A phased rollout or additional experimentation is recommended.

---

# Assumptions and Limitations

## Assumptions

* The dataset accurately represents user behavior.
* Experiment groups were randomly assigned.
* All binary variables contain valid values.
* Revenue values are correctly recorded.

## Limitations

* Results are based on a single experiment.
* Long-term customer retention was not evaluated.
* External business factors were not considered.
* Additional experiments may be required before a full rollout.

---

# Screenshots Included

* summary_metrics.png
* hypothesis_test_output.png
* kpi_tree_preview.png
