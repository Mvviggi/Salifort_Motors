 # **Capstone project: Providing data-driven suggestions for HR**   


The dataset that used in this capstone contains 15,000 rows and 10 columns for the variables listed below. 

**Note:** The dataset source was downloaded from [Kaggle](https://www.kaggle.com/datasets/mfaisalqureshi/hr-analytics-and-job-prediction?select=HR_comma_sep.csv).

Variable  |Description |
-----|-----|
satisfaction_level|Employee-reported job satisfaction level [0&ndash;1]|
last_evaluation|Score of employee's last performance review [0&ndash;1]|
number_project|Number of projects employee contributes to|
average_monthly_hours|Average number of hours employee worked per month|
time_spend_company|How long the employee has been with the company (years)
Work_accident|Whether or not the employee experienced an accident while at work
left|Whether or not the employee left the company
promotion_last_5years|Whether or not the employee was promoted in the last 5 years
Department|The employee's department
salary|The employee's salary (U.S. dollars)

-------------------------------------------------------------------------------------------------------------

 ### Plan Stage
1. The main stakeholders are Salifort’s senior leadership team and the Human Resources department.
2. Analyze the survey data taken by employees and come up with ideas for how to increase employee retention. 
3. Employees from the Sales department were the most that took the survey out of 10 departments in the company.
4. Used Excel Pivot Table for a first glance of the data, and then used the dataset in Visual Studio Code for all EDA, Construct, and Execute phase.
5. Given this dataset was provided by Coursera and created for a fictional company, it can be assumed it reliability and originality.

#### Analyze Stage 
Summary of EDA performed:
1. Removed duplicates
2. Check for outliers: tenure column had 824 rows
3. The satisfactory level column ranges from 0.09 to 1.0.
4. The tenure column ranges from 2 to 10 years, with a median of 3 years.
5. Some columns had mix of upperclass letters which were all converted to lowercase. The column orginally called 'time_spend_company' was changed to 'tenure' for simple and concise name.
6. EDA process: <br>
    a. Get more understanding of employees staying vs leaving the company. <br>
    b. Create data visualizations to evaluate relationships between independent and dependent variables.
7. Results indicate that 16% of employees left while 83% of employees stayed at the company.

Some EDA visualization:
![Counts of survey forms submtted by Department](departmentcount.png)

Correlation Heatmap
![Columns Correlation Heatmap](correlationheatmap.png)
The heatmap above shows that the employees that left the company correlated negatively with satisfaction_level. Meanwhile, the number of projects, average monthly hours and  evaluation scores had a positive correlation with each other. 