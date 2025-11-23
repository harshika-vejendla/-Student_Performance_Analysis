Student Performance Analysis

A Data Analytics Case Study using Python, Seaborn & Statistical Testing

1. Project Overview

This project analyzes academic performance of 1,000 students across Math, Reading, and Writing, to understand how demographics, test preparation, socio-economic factors, and parental education impact learning outcomes.

The study uses Python for:

Data cleaning

Feature engineering

Exploratory data analysis

Data visualization

Statistical testing (t-test)

2. Dataset Summary

The dataset contains:

gender

race/ethnicity

parental level of education

lunch type (standard, free/reduced)

test preparation course (completed / none)

math score

reading score

writing score

Derived features created:

total score = math + reading + writing

average score = total score / 3

 3. Tools & Technologies Used

Python: pandas, numpy

Visualization: seaborn, matplotlib

Statistics: scipy.stats (t-test)

Environment: Jupyter Notebook

 4. Analysis Performed
✔ Data Loading & Cleaning

Loaded CSV with pandas

Checked dtypes, non-null counts

Computed summary statistics

No missing values found

Created total and average score columns

✔ Exploratory Data Analysis (EDA)

Gender distribution

Score distributions (math/reading/writing)

Boxplot: test preparation vs average score

Race × Gender vs Average Score

Parental education vs Average Score

Lunch type × Gender vs Average Score

✔ Statistical Test

Independent two-sample t-test to evaluate whether completing test preparation significantly increases average scores.

5. Business Findings & Insights

Based entirely on the results and charts inside the notebook.

1. Test preparation significantly boosts performance

Students who completed the test preparation course score notably higher than those who didn’t.

p-value < 0.05 → statistically significant

Difference is real, not due to randomness

Business Impact:
Schools should invest in or require structured test preparation programs to improve academic outcomes.

2. Lunch type strongly correlates with performance

Students with standard lunch consistently outperform those with free/reduced lunch across genders.

Interpretation:
Lunch type is a strong proxy for socio-economic status (SES).

Business Impact:
Schools should target:

Supplementary coaching

Nutrition support

After-school programs
for socio-economically disadvantaged students.

3. Parental education level directly impacts student performance

Higher parental education (associate, bachelor’s, master’s) is linked to higher average scores.

Business Impact:
Policymakers should:

Develop family education workshops

Engage parents in literacy programs

Provide additional student mentoring for lower-education households

4. Race/Ethnicity shows performance variation

Your visualizations show:

Group E and Group C students perform highest

Group A generally underperforms

Within several groups, females outperform males

Business Impact:
Interventions should focus on:

Resource distribution

Curriculum support

Equity-focused academic programs

 5. Gender performance patterns are subject-specific

Females score higher in reading and writing

Math scores are more balanced across genders

Business Impact:
Teachers can tailor:

Reading/writing encouragement for boys

Math confidence-building for girls