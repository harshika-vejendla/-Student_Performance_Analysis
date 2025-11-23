# 🎓 Student Performance & Achievement Analysis

## 📖 Project Overview
This project analyzes the key factors influencing student performance, including socio-economic background, parental education, and test preparation. Moving beyond basic visualizations, this analysis employs **statistical hypothesis testing** and **feature engineering** to derive scientifically backed conclusions about educational equity and achievement gaps.

---

## ❓ Business Problem & Objectives
Educational institutions often struggle to identify which interventions (like test prep courses or lunch subsidies) yield the most significant improvements in student scores.
This analysis aims to answer:
1.  **Effectiveness:** Does the "Test Preparation Course" actually lead to statistically significant score improvements?
2.  **Equity:** How do socio-economic factors (Lunch Type) and Parental Education impact student success?
3.  **Subject Gaps:** Are students performing consistently across Math, Reading, and Writing, or are there significant "skill gaps"?

---

## 📂 The Dataset
* **Source:** Student Performance Dataset.
* **Size:** 1,000 records.
* **Key Features:**
    * `math score`, `reading score`, `writing score`: Numerical performance metrics.
    * `test preparation course`: Completed vs. None.
    * `parental level of education`: Bachelor's, Master's, High School, etc.
    * `lunch`: Standard vs. Free/Reduced (a proxy for socio-economic status).
    * `race/ethnicity`: Demographic groups (Group A - E).

---

## 🛠️ Methodology & Tech Stack

### **Technologies Used**
* **Python**: Core analysis.
* **Pandas & NumPy**: Data manipulation and aggregation.
* **Seaborn & Matplotlib**: Advanced visualization (Distribution plots, Heatmaps, Box plots).
* **SciPy (`scipy.stats`)**: For statistical hypothesis testing (T-tests).

### **Key Analysis Steps**
1.  **Feature Engineering**:
    * Created `total score` and `average score` metrics.
    * Developed `math_reading_gap` to identify lopsided skill sets.
    * Generated `performance_band` (Low/Medium/High) to categorize student achievement levels.
2.  **Statistical Testing**:
    * Performed an **Independent T-Test** to verify if the difference in scores between students who took the test prep course vs. those who didn't was statistically significant (p-value < 0.05).
3.  **Multivariate Analysis**:
    * Analyzed the interaction between Gender, Race, and Test Prep on average scores.

---

## 💡 Key Findings & Insights

### **1. The "Test Prep" Advantage (Statistically Proven)**
* **Finding:** Students who completed the test preparation course scored significantly higher than those who did not.
* **Statistical Evidence:** The T-Test yielded a **p-value < 0.05**, rejecting the null hypothesis. This confirms that the score improvement is real and not just due to random chance.
* **Actionable Insight:** Schools should prioritize funding and access to test preparation courses, as they are a proven lever for performance improvement.

### **2. The "Lunch Gap" (Socio-Economic Impact)**
* **Finding:** Students with "Standard" lunch consistently outperformed those with "Free/Reduced" lunch across all subjects.
* **Insight:** Socio-economic status is a strong predictor of academic performance. Interventions must go beyond the classroom (e.g., nutritional support, after-school tutoring) to bridge this equity gap.

### **3. Parental Education Correlation**
* **Finding:** There is a clear positive correlation between parental education level and student scores. Students whose parents hold a Master's degree achieved the highest median scores.
* **Insight:** First-generation students or those from lower-education households may require additional mentorship programs to compete on level ground.

### **4. Subject Skill Gaps**
* **Finding:** Math scores showed a wider variance compared to Reading and Writing.
* **Insight:** Math appears to be the most "polarizing" subject, suggesting a need for targeted remedial math programs for the lower-performing cohort.

---

## 📊 Visualizations
The analysis includes the following professional charts:
* **Score Gap Box Plots:** Visualizing the disparity between Math and Reading/Writing skills.
* **Correlation Heatmap:** Showing the strong relationship between Reading and Writing scores.
* **Distribution Plots:** Histograms showing the bell-curve distribution of scores.
* **Grouped Bar Charts:** Comparing performance by Gender and Lunch type.

---

