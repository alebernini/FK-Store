# 📊 FK Store - A/B Test Analysis and Hypothesis Prioritization

## 📝 Project Description

In collaboration with the marketing department, you’ve compiled a list of hypotheses that could potentially increase revenue. The task is to prioritize these hypotheses, conduct an A/B test, and analyze the results to support decision-making.

## 📁 Datasets
Part 1: Hypothesis Prioritization
/datasets/hypotheses_us.csv

Hypothesis — Short descriptions of each hypothesis.

Reach — User reach on a scale from 1 to 10.

Impact — Expected impact on users (1–10).

Confidence — Confidence in the hypothesis (1–10).

Effort — Resources required to test the hypothesis (1–10). Higher values mean more resources needed.

Part 2: A/B Test Analysis
/datasets/orders_us.csv

transactionId — Unique order identifier.

visitorId — Unique visitor identifier.

date — Date of the order.

revenue — Revenue from the order.

group — A/B test group (A or B).

/datasets/visits_us.csv

date — Date of visit.

group — A/B test group.

visits — Number of visits per group per day.

⚠️ Note: Please pre-process the datasets. There may be inconsistencies, such as visitors appearing in both groups A and B.

🚦 Part 1: Hypothesis Prioritization
The file hypotheses_us.csv contains nine hypotheses aimed at increasing the store’s revenue. Each hypothesis includes the Reach, Impact, Confidence, and Effort values.

Tasks:
Apply the ICE framework to prioritize hypotheses. Rank them in descending order.

Apply the RICE framework to prioritize hypotheses. Rank them in descending order.

Compare ICE vs RICE results and explain the differences in prioritization.

🧪 Part 2: A/B Test Analysis
Analyze the results from the A/B test using orders_us.csv and visits_us.csv.

Tasks:
Cumulative Revenue:

Plot cumulative revenue by group.

Draw conclusions and make hypotheses.

Average Order Value:

Plot cumulative average order value by group.

Draw conclusions and make hypotheses.

Relative Difference in AOV:

Plot relative difference in cumulative AOV for group B compared to group A.

Draw conclusions and make hypotheses.

Daily Conversion Rate:

Calculate and plot daily conversion rate (orders/visits) for each group.

Draw conclusions and make hypotheses.

Relative Conversion Difference:

Plot relative difference in cumulative conversion rate for group B vs. A.

Draw conclusions and make hypotheses.

Outliers in Orders per User:

Calculate the 95th and 99th percentiles for number of orders per user.

Define thresholds for anomalies.

Order Price Distribution:

Plot a scatter chart of order prices.

Draw conclusions and make hypotheses.

Outliers in Order Prices:

Calculate the 95th and 99th percentiles for order values.

Define thresholds for anomalies.

Statistical Significance (Raw Data):

Assess statistical significance of conversion rate difference between groups.

Assess statistical significance of AOV difference between groups.

Draw conclusions and make hypotheses.

Statistical Significance (Filtered Data):

Filter out anomalies based on thresholds.

Reassess statistical significance of conversion and AOV differences.

Draw conclusions and make hypotheses.

Final Decision:

Based on your findings, choose one of the following actions:

Stop the test, declare a leading group.

Stop the test, no significant difference.

Continue the test.

## 🛠️ Tools & Technologies
Python (Pandas, Matplotlib, Seaborn, SciPy)

Jupyter Notebook

A/B Testing

Statistical Analysis

Data Preprocessing & Cleaning

## 📌 Objectives
Learn and apply hypothesis prioritization frameworks (ICE, RICE).

Conduct a robust A/B test analysis.

Interpret statistical results to make business decisions.

## ✅ Conclusion
The p-value for the conversion rate comparison between groups A and B was less than 0.05, allowing us to reject the null hypothesis that there is no difference between the two groups.
Moreover, group B showed a conversion improvement greater than 10%, indicating a meaningful and promising impact. Therefore, the strategy applied to group B appears to deliver better performance and higher results.

However, there is no statistically significant difference in the average order value between the groups, as the p-value for this metric was 1.000.
This suggests that while the number of conversions increased, the size of individual orders remained the same.

