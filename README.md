# Customer_Engagement_Analysis-Excel
This project focuses on analyzing the impact of adding new features to the 365 Data Science platform using Q4 user data across 2021-2022.
**Tools**: Excel.
**Skills**: Exploratory Data Analysis (EDA), summary statistics, inferential statistics, hypothesis testing, statistical testing using f-tests, t-tests, and p-values, translating data to business insights, and data storytelling.
**Outputs**: 
  * Excel worksheet where each tab focuses on a particular calculation and specific insights garnered from those calculations.
  * Presentation slides including objectives, key metrics, hypothesis (business question), key findings, regional analysis, business implications, and recommendations. 

# 📊 Student Engagement Analysis – Q4 2021 vs Q4 2022
We use masked user data to investigate whether engagement levels (measured in minutes watched) increased from Q4 2021 to Q4 2022 among free-plan and paid-plan students on the 365 Data Science platform. The goal is to use data-driven analysis to support strategic decisions about product features and market focus.

## 📁 Project Structure

- `Engagement Project.xlsx`: Raw and processed engagement data
  * Includes data for free and paid-plan students in Q4-2021 and Q4-2022
  * And data of free-plan students from India and the US in 2022
- `README.md`: Project report and summary

## 🎯 Objective
To determine if engagement levels significantly increased after new platform features were introduced, by comparing Q4 2021 and Q4 2022 watch-time for both:
- Free-plan students
- Paid-plan students

Additionally, to compare engagement between free-plan students in India and the US.

## 🎲 Dataset Structure
### Columns
  1. `student_id` – a unique identifier for each student in the dataset.
  2. `paid` - binary variable indicating whether a student had a paid account during that time.
  3. `minutes_watched_21` - represents a student's engagement level during Q4-2021
  4. `minutes_watched_22` - represents a student's engagement level during Q4-2021

The dataset is available on the 365 Data Science platform under Course Projects. 

## 🔬 Methods Used
### 1. Descriptive Statistics
- Mean, Median, Standard Deviation
- Skewness and Kurtosis for distribution shape

### 2. Confidence Intervals
- 95% CI using Z-statistic (due to large n)
- 
### 3. Hypothesis Testing
- **Null Hypothesis** (H₀): Engagement in Q4 2021 ≥ Engagement in Q4 2022
- **Tests Used**:
  - Two-sample t-test (assuming unequal variances)
  - F-test to confirm variance inequality

### 4. Regional Comparison
- US vs India (free-plan students only)
- **Null Hypothesis** (H₀): US engagement ≥ India
- 
## 🖼️ Data Analysis Summary
  1. Both free and paid users had a noticeable increase in watch time from Q4-2021 to Q4-2022, with paid users having an **over 700% increase** in watch time. However, the data showed extreme skewness and kurtosis, especially in 2022, implying that a small group of focused users were responsible for the high average watch time. High standard deviation in Q4-2022 and relatively similar median values across the board support this conclusion.
  2. Despite skewed raw data, the large sample sizes allow us to use the z-statistic method, so normality was assumed for confidence interval estimation and hypothesis testing. Confidence interval calculations showed that paid plan users had a statistically significant increase in engagement, while free plan users had a drop in engagement.
  3. We reject the first null hypothesis (2021 engagement is ≥ 2022 engagement) for _paid plan students_ as the t-statistic is lower than the critical value. We fail to reject the same hypothesis for _free plan students_ as the calculated t-stat is higher than the critical value. These results align with our previous findings.
  4. We fail to reject the second null hypothesis (US engagement is ≥ India engagement)

**Note**: Rejecting a null hypothesis does not prove the alternative hypothesis is true

## 📌 Conclusion
The analysis supports that student engagement (minutes watched) significantly increased in Q4 2022 for free but particularly for paid users, suggesting that new platform features may have contributed to this. However, there is not enough data to make a proper conclusion about the difference between US and Indian free-plan students.

## 🔍 Future Analysis Opportunities
- Analyze engagement by feature
- Control for outliers
- Analyze by segment


