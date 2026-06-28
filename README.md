# Task 1: Business Problem Statement

The company has introduced a new onboarding and activation campaign for new users. An A/B experiment was conducted by dividing users into two groups: a **Control Group**, which experienced the existing onboarding process, and a **Treatment Group**, which experienced the new onboarding campaign.

The primary business decision is to determine whether the new onboarding experience should be launched to all users based on its performance.

This decision impacts business leadership, the product team, the marketing team, and future users of the platform.

The primary metric expected to improve is the **Paid Conversion Rate**, as increasing the number of users who become paying customers directly supports business growth and revenue.

Before making a final recommendation, it is also important to monitor potential risks such as increased refund requests, higher support ticket rates, lower engagement scores, and longer conversion times. An improvement in conversion alone is not sufficient if it negatively affects user experience or revenue quality.

The final recommendation should therefore be supported by experiment results, hypothesis testing, comparison of key performance metrics, and evaluation of guardrail metrics to ensure that the treatment delivers sustainable business value.


# Task 2: North Star Metric

## Selected North Star Metric

**Paid Conversion Rate**

### Why this is the North Star Metric

Paid Conversion Rate is the most important success metric because it directly measures how many users become paying customers after experiencing the onboarding process. Since the company's objective is to increase subscriptions and revenue, this metric best represents the success of the new onboarding campaign.

### Why Other Metrics Are Supporting Metrics

The following metrics help explain user behaviour but do not directly represent business success:

* Landing Page Visit Rate measures initial interest.
* Trial Start Rate measures user activation.
* Onboarding Completion Rate measures onboarding effectiveness.
* Average Revenue Per User measures revenue performance.
* Engagement Score measures user activity.
* Refund Rate and Support Ticket Rate monitor customer experience and potential risks.

These metrics support decision-making but ultimately contribute to improving the Paid Conversion Rate.

### Connection to Business Growth

An increase in Paid Conversion Rate leads to:

* Higher subscription revenue.
* Better customer acquisition efficiency.
* Improved return on marketing investment.
* Sustainable long-term business growth.

### Risk of Optimizing Only This Metric

Focusing only on Paid Conversion Rate may create unintended problems. Users might convert initially but later request refunds, raise more support tickets, show lower engagement, or churn quickly. Therefore, guardrail metrics such as Refund Rate, Support Ticket Rate, Engagement Score, and Days to Convert must also be monitored before making the final business recommendation.



## Task 4: Data Preparation

The experiment dataset was reviewed and prepared before analysis.

### Data Quality Checks Performed

- Checked missing values across all columns.
- Missing values in categorical columns (such as device_type and traffic_source) were filled with "Unknown".
- Missing engagement_score values (14 records) were imputed using the median value (59.9).
- Missing days_to_convert values were retained because they represent users who did not convert.
- Verified experiment group counts (Control: 693, Treatment: 715).
- Checked duplicate user IDs and identified 16 duplicate records. These were retained because no business rule required their removal.
- Verified binary fields (visited_landing_page, started_trial, completed_onboarding, converted_to_paid, and refund_requested). All contained only valid values (0 and 1).
- Reviewed revenue_30d values for abnormal outliers. No unrealistic values requiring treatment were identified.
- Reviewed region distribution across Control and Treatment groups. The distribution was reasonably balanced for comparison.
