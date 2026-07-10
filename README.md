
Student Performance Factors — Data Analysis

A data analysis project exploring the Student Performance Factors dataset using Python (Pandas & NumPy) to understand what drives exam performance and improvement.

Dataset from Kaggle dataset
StudentPerformanceFactors.csv — 6,607 student records with 20 columns

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
-
- <img width="640" height="480" alt="Improvment_Status" src="https://github.com/user-attachments/assets/b76370b5-09bb-422a-9379-53271765dc6a" />

- **Peer Influence**: students with positive peer influence average 67.62, vs. 67.20 (neutral) and 66.56 (negative) — a small but consistent ~1-point gap.

<img width="640" height="480" alt="Peer Influence vs Average Exam Score" src="https://github.com/user-attachments/assets/be10aaec-0935-49fe-8797-75ea0a740770" />

**Sleep Hours** : the Exam Scorce of students are quite simliar for all sleeping hours

<img width="640" height="480" alt="Sleep Hours vs Exam Score" src="https://github.com/user-attachments/assets/1affb6b1-4802-443b-862f-d263cd662a7a" />
