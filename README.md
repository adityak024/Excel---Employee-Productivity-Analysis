# Excel---Employee-Productivity-Analysis
This project provides an Excel-based solution for analyzing employee productivity using structured data, formulas, and visual dashboards. The goal is to help managers and HR teams track performance metrics, identify high-performing employees, and make data-driven decisions to improve workforce efficiency.
This Excel project analyzes employee performance using various productivity metrics and advanced Excel functions. It is designed to help HR teams and managers make data-driven decisions based on trends, efficiency, and performance indicators.

🔧 Features & Functions Used
Sorting & Filtering: Organized and segmented employee data based on department, performance, and efficiency.

Bar Charts: Visualized key performance indicators like Tasks Completed, Hours Worked, and Ratings.

Standard Deviation: Measured performance consistency within departments using the STDEV.P function.

PivotTables: Summarized data by Department and calculated variations in performance.

Ranking: Employees were ranked by Performance Efficiency Index (PEI) to identify top performers.

CORREL Function: Used to analyze relationships between variables like Hours Worked and Tasks Completed.

Logical Analysis: Applied IF, FILTER, AVERAGE, MAX, INDEX-MATCH, and XLOOKUP for targeted insights.

📌 Key Analysis Performed
✅ 1. Least Variation in Performance by Department
Used STDEV.P in a PivotTable grouped by Department.

Identified which departments had the most consistent employee performance.

🥇 2. Top 3 Employees Based on PEI
Ranked all employees by their Performance Efficiency Index (PEI).

Used SORT, LARGE, and INDEX-MATCH to extract and display the top 3 performers.

📈 Correlation Analysis
Q1: What influences Performance Rating more – Hours Worked or Tasks Completed?
Used =CORREL() to compare correlation coefficients:

CORREL(Performance_Rating, Hours_Worked)

CORREL(Performance_Rating, Tasks_Completed)

Interpreted which variable had a stronger relationship with performance.

Q2: Work Hours and Productivity Correlation
Created a scatter plot to visualize the correlation between:

Hours_Worked and Productivity_Score

Analyzed the direction of the correlation (positive or negative).

🌟 Special Insights
Underutilized High Performers
Identified employees who:

Have a Performance Rating ≥ 4, and

Worked less than the average hours (AVERAGE(Hours_Worked))

Used:

excel
Copy
Edit
=FILTER(Employee_List, (Performance_Rating>=4)*(Hours_Worked<AVERAGE(Hours_Worked)))
These employees are potential efficient but underutilized performers.

⏱️ Tasks per Hour Efficiency
Added a custom column:

excel
Copy
Edit
=Tasks_Completed / Hours_Worked
Used MAX, INDEX-MATCH, or XLOOKUP to find:

The most task-efficient employee.

Their department, productivity score, and rating.

📂 Project Files
EmployeeProductivityAnalysis.xlsx – Main Excel workbook with all data and analysis.

Charts_and_Pivot_Tables.pdf – Exported visuals for presentation use.

README.md – This file.

💡 Conclusion
This analysis uncovers actionable insights such as:

Top performers by efficiency

Departments with stable performance

Underutilized but valuable employees

Variables most correlated with performance outcomes
