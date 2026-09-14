# Projects

## Student Performance Analysis

### Research Question

How do study time, absences, and previous class failures relate to students' final math grades?

### Project Overview

This project analyzes student performance data from the UCI Machine Learning Repository. The goal is to explore whether study habits, school absences, and previous class failures are related to students' final mathematics grades.

### Dataset

The dataset contains information on 395 students and 33 features. Each row represents one student in a Portuguese secondary school mathematics course.

The dataset includes demographic information, study habits, absences, previous class failures, and grades. For this analysis, I focused on:

- **Study Time:** Weekly study time reported in four categories
- **Absences:** Number of school absences
- **Previous Failures:** Number of previous class failures
- **Final Grade (G3):** Final mathematics grade on a 0–20 scale

The dataset contained no missing values, so no observations needed to be removed or imputed.

### Methods

I used Python, pandas, matplotlib, and scikit-learn to analyze the data.

The analysis included:

- Exploratory data analysis
- Data cleaning and preparation
- Bar charts and scatter plots
- Correlation analysis
- Linear regression
- Logistic regression
- Decision tree classification

### Key Findings

Previous class failures showed the clearest relationship with final math grades. Students with more previous failures generally had lower average final grades.

Study time showed a small positive relationship with final grades. Students who reported more study time generally had slightly higher average grades, but the difference between study-time groups was not large.

Absences showed very little linear relationship with final grade in this dataset.

The linear regression model had an R² of approximately **0.03**, showing that these three variables alone explained only a small amount of the variation in final grades.

For classification, logistic regression achieved approximately **73.4% accuracy**, while the decision tree achieved approximately **75.9% accuracy**. The decision tree performed slightly better.

### Limitations

The dataset only represents students from two Portuguese secondary schools, so the results may not generalize to all students.

The analysis also focuses on only three predictors. Other factors, such as motivation, family support, teaching quality, socioeconomic background, and access to academic resources, could affect student performance.

Because the data are observational, the results show relationships between variables but cannot prove that any of these factors directly cause changes in grades.

### Code

[View the Full Jupyter Notebook](student_performance_analysis.ipynb)

### Dataset Source

Cortez, P. (2008). *Student Performance* [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5TG7T

### References

Aucejo, E. M., & Romano, T. F. (2016). Assessing the effect of school days and absences on test score performance. *Economics of Education Review, 55*, 70–87. https://doi.org/10.1016/j.econedurev.2016.08.007

Nonis, S. A., & Hudson, G. I. (2010). Performance of college students: Impact of study time and study habits. *Journal of Education for Business, 85*(4), 229–238. https://doi.org/10.1080/08832320903449550

Plant, E. A., Ericsson, K. A., Hill, L., & Asberg, K. (2005). Why study time does not predict grade point average across college students: Implications of deliberate practice for academic performance. *Contemporary Educational Psychology, 30*(1), 96–116. https://doi.org/10.1016/j.cedpsych.2004.06.001
