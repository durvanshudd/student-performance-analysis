Student Performance Factors — Data Analysis

A data analysis project exploring the Student Performance Factors dataset using Python (Pandas & NumPy) to understand what drives exam performance and improvement.

Dataset
StudentPerformanceFactors.csv — 6,607 student records with 20 columns, including:

Tools & Libraries:
Python
Pandas
NumPy

What the notebook does

Data cleaning — loads the CSV, checks for null values, and drops duplicate rows.
Top & bottom performers — finds the highest and lowest scorer in the recent exam, plus the top 10 and bottom 10 lists by Exam_Score.
Improvement tracking — creates a Diffrence In Exam_Scores column (Exam_Score - Previous_Scores) and an Improvment_Status column.

Then counts how many students fall into each category, and identifies the students with the biggest improvement and the biggest decline.
Overall average — calculates the class average exam score.
Relationship analysis — uses groupby() + value_counts() / mean() to explore how Improvment_Status and Exam_Score relate to:

Physical activity
Internet access
Sleep hours
Learning disabilities & motivation level
Family income & access to resources
Teacher quality & school type
Peer influence

# Results

**Overall performance**
- 65.6% of students (4,332 of 6,607) showed an *Improvement Decline* from their previous exam, 32.4% improved, and only 2% stayed the same.

**Factors with a MAJOR on Exam Score**
- **Peer Influence**: students with positive peer influence average 67.62, vs. 67.20 (neutral) and 66.56 (negative) — a small but consistent ~1-point gap.
- **Teacher Quality**: students with high-quality teachers average 67.68 vs. 66.75 for low-quality — also a small but consistent ~1-point gap.

**Factors with little to no effect**
- **Internet Access**: improvement-decline rate is nearly identical with internet (65.5%) vs. without (66.5%), and average sleep hours barely differ (7.03 vs. 6.97) — internet access doesn't meaningfully affect either outcome in this dataset.
- **Learning Disabilities vs. Motivation Level**: near-identical distribution regardless of learning disability status .
- **Family Income vs. Access to Resources**: surprisingly flat — Low, Medium, and High income students report similar resource access across all levels
- **Teacher Quality vs. School Type**: no link 70% of students are in public school regardless of teacher-quality rating.
