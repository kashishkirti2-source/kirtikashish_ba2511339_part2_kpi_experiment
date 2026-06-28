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
