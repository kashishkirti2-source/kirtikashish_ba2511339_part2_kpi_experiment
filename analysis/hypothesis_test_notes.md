# Task 6: Hypothesis Test Notes

## Metric Being Tested

Paid Conversion Rate

## Reason for Choosing This Metric

Paid Conversion Rate is the most important business metric because it directly measures how many users become paying customers. The goal of the experiment is to determine whether the treatment increases paid subscriptions compared to the control group.

## Null Hypothesis (H0)

There is no significant difference in the paid conversion rate between the Control group and the Treatment group.

**H0:** Conversion Rate (Treatment) = Conversion Rate (Control)

## Alternative Hypothesis (H1)

The paid conversion rate of the Treatment group is significantly higher than that of the Control group.

**H1:** Conversion Rate (Treatment) > Conversion Rate (Control)

## Type of Test

One-tailed test

## Significance Level

α = 0.05 (5%)

## Interpretation Logic

* If the p-value is less than 0.05, reject the null hypothesis and conclude that the Treatment significantly improves the paid conversion rate.
* If the p-value is greater than or equal to 0.05, fail to reject the null hypothesis and conclude that there is not enough evidence to show the Treatment improves the paid conversion rate.

## Business Decision

If the Treatment group shows a statistically significant increase in paid conversion rate, the new experiment should be rolled out to all users. Otherwise, the current experience should be retained or the experiment should be revised before deployment.




# Task 7: Hypothesis Test Analysis

## Test Used
Chi-Square Test of Independence

## Primary Metric
Paid Conversion Rate

## Test Inputs

| Group | Converted | Not Converted | Total |
|-------|-----------|---------------|------:|
| Control | 22 | 671 | 693 |
| Treatment | 50 | 665 | 715 |

## Significance Level
α = 0.05

## Test Output

P-value = 0.001146

## Decision Rule

- If p-value < 0.05 → Reject Null Hypothesis.
- If p-value ≥ 0.05 → Fail to Reject Null Hypothesis.

## Result

Since p-value (0.001146) is less than 0.05, the null hypothesis is rejected.

## Business Interpretation

The treatment group achieved a significantly higher paid conversion rate than the control group. This indicates that the experimental treatment positively influenced user conversions and should be considered for implementation.


# Task 8: Guardrail Metrics Evaluation

The treatment group increased paid conversions, but additional guardrail metrics were evaluated before making a business recommendation.

## 1. Refund Rate
- Control: 0.00%
- Treatment: 0.42%

The treatment group showed a small increase in refund requests. However, the refund rate remains very low and does not currently present a major business risk.

## 2. Support Ticket Rate
- Control: 21.93%
- Treatment: 37.20%

Support ticket rate increased noticeably in the treatment group. This suggests users required more assistance, which may increase operational costs and indicate usability issues. This is an important risk that should be monitored.

## 3. Average Days to Convert
- Control: 8.86 days
- Treatment: 6.40 days

Users in the treatment group converted faster than the control group. This is a positive outcome and reduces the customer acquisition cycle.

## 4. Average Engagement Score
- Control: 57.05
- Treatment: 62.90

Engagement improved in the treatment group, suggesting that users interacted more actively with the product.

## 5. Revenue Quality
- Average Revenue per Converted User
  - Control: 1630.10
  - Treatment: 770.41

Although conversions increased, revenue generated per converted user decreased. This indicates a potential decline in revenue quality and should be investigated before a full rollout.

## Overall Assessment

While the treatment significantly improved paid conversion rate, the increase in support tickets and the decline in revenue per converted user indicate potential risks. A phased rollout with further investigation is recommended rather than an immediate full deployment.
