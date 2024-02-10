# HR-ANALYTICS-DASHBOARD
This repository contains a HR Analytics Power BI dashboard designed to analyze and visualize employee attrition data within a company. The dashboard provides comprehensive insights into factors influencing attrition rates and potential areas for intervention to improve employee retention.


## Problem Statement

Employee attrition can have significant impacts on organizational performance, productivity, and morale. High attrition rates not only result in the loss of valuable talent but also incur costs associated with recruitment, training, and productivity loss. The problem statement revolves around understanding the factors contributing to employee attrition and developing strategies to mitigate attrition rates within the organization.

### Objective: 
To Identify key factors influencing employee attrition within the organization. Develop actionable insights to inform retention strategies and reduce attrition rates.


## Steps Followed 

- Step 1 : Load data into Power BI Desktop using get data, import text/csv since our data file is csv file.
- Step 2 : After loading data or while importing only click on Transform data, Power Query Editor is opened. 
- Step 3 : Explore the data set and understand each attribute. Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset" in the bottom left

    - Age  : Employee's age. 
    - Attrition: Whether the employee has attrited (Yes/No).
    - BusinessTravel: Frequency of business travel (e.g., Travel_Rarely, Travel_Frequently).
    - DailyRate: Daily rate of pay.
    - Department: Department where the employee works.
    - DistanceFromHome: Distance of employee's residence from the workplace.
    - Education: Level of education attained.
    - EducationField: Field of education.
    - EmployeeCount: Number of employees (constant value in this dataset).
    - EmployeeNumber: Unique identifier for each employee.
    - EnvironmentSatisfaction: Satisfaction level with the work environment.
    - Gender: Employee's gender.
    - HourlyRate: Hourly rate of pay.
    - JobInvolvement: Level of job involvement.
    - JobLevel: Employee's job level within the organization.
    - JobRole: Role or position of the employee.
    - JobSatisfaction: Level of job satisfaction.
    - MaritalStatus: Marital status of the employee.
    - MonthlyIncome: Monthly income.
    - MonthlyRate: Monthly rate of pay.
    - NumCompaniesWorked: Number of companies the employee has worked for.
    - Over18: Indicates whether the employee is over 18 years old (Y/N).
    - OverTime: Indicates whether the employee works overtime (Yes/No).
    - PercentSalaryHike: Percentage of salary hike.
    - PerformanceRating: Performance rating.
    - RelationshipSatisfaction: Satisfaction level with work relationships.
    - StandardHours: Standard number of working hours (constant value in this dataset).
    - StockOptionLevel: Level of stock options.
    - TotalWorkingYears: Total number of years the employee has worked.
    - TrainingTimesLastYear: Number of training sessions attended last year.
    - WorkLifeBalance: Work-life balance satisfaction.
    - YearsAtCompany: Number of years the employee has worked at the current company.
    - YearsInCurrentRole: Number of years in the current role.
    - YearsSinceLastPromotion: Number of years since the last promotion.
    - YearsWithCurrManager: Number of years with the current manager.
- Step 4 : Clean and Transform the data.

  1 . Check the data type of each column and Convert to required data type if necessary.

  2 . Handling null values - In view tab under Data preview section, check "column distribution", "column quality" & "column profile" options. From the column quality empty percentage we know if any null values are present. In our dataset there are no null values.

  3 . Handling Duplicates - Check for duplicate record and remove them if necessary, ensure that it won’t effect the analysis.

  4 . Handling Inconsistent data - Look for variations in categorical data and Standardize them to ensure consistency

  5 . Create a new column named "Attrition_Count" that contains the count of people who have left, represented as 1 for "Yes" and 0 for "No" using Conditional column from Add Column tab.

    Close and apply to apply changes and load the transformed data into Power BI.

- Step 5 : Navigate to Report View and design Visualizations.

  1 . Card visuals were added to the canvas to represent the key performance indicators - count of employees, employees left, attrition rate, average salary, average age, average years worked .

  2 . Created a donut chart to find the attribute by education filed. It is observed that the attrition rates are highest in Life sciences, followed by medical, marketing, technical degree.

  3 . Created a donut chart to assess attrition rates based on work-life balance ratings, revealing a predominant proportion in the moderate balance category (Rating 3, 54%), while drill-down shows varying job satisfaction ratings, with the highest dissatisfaction observed in Rating 1 (28%).

  4 . Created a line chart depicting attrition counts by age and marital status, showing a trend where the attrition count is higher among married individuals, followed by singles and divorced, with a peak observed between the ages of 30 to 40.

  5 . Generated a stacked column chart illustrating attrition counts by percent salary hike, showcasing the highest attrition count for salary hikes between 10 to 15 percent.

  6 . Created a stacked bar chart representing attrition counts by job role, where attrition counts are highest for lab technicians (62), followed by sales executives (57), research scientists (47) and sales representative (33) with other roles having lower attrition counts.

  7 . Created a stacked bar chart displaying attrition status on the x-axis and average years at current company, in current role, and with current manager on the y-axis. Employees experiencing higher attrition rates have lower average years spent in their current company, role, and with their current manager.

  8 . Created Slicers for department and gender category.


# Snapshot of Dashboard 

![snap](https://github.com/navyarmadireddy/HR-ANALYTICS-DASHBOARD/assets/122340189/436169e2-d4c6-4d8f-b561-d48b0c4d84ce)



# Insights

Following inferences can be drawn from the dashboard;

### [1] Departmental Analysis:

- Human Resources: The Human Resources department exhibits relatively low attrition rates, suggesting a stable workforce. But faces challenges in work life balance.
    - Actions: Investigate the factors contributing to employee satisfaction and retention within this department to identify best practices that can be applied elsewhere. Review and enhance work life balance initiatives.
- Research and Development: Attrition rates in the Research and Development department appear moderate, indicating potential areas for improvement in employee engagement or career development opportunities.     
    - Actions: Conduct surveys or focus groups to understand employee concerns and implement targeted interventions to enhance retention.
- Sales: The Sales department experiences higher attrition rates compared to other departments, indicating potential challenges in retention. 
    - Actions: Develop strategies to address factors contributing to turnover, such as workload, compensation, or job satisfaction, to improve employee retention and performance.

### [2] Gender Analysis:

- Men experience slightly higher attrition rates predominantly in the Laboratory Technician role.
- Women exhibit a moderate attrition rate primarily in the Sales Executive role.
    - Actions: Assess the job satisfaction, workload, and growth opportunities in Sales Executive and Laboratory Technician roles, implementing targeted interventions to enhance job satisfaction
           
### [3] Age and Tenure Analysis:

- Employees between the ages of 30 to 40 exhibit a peak in attrition, indicating a critical period for retention efforts. 
    - Actions: Develop career advancement opportunities, mentorship programs, and flexible work arrangements to support employees during this career stage and reduce turnover.
- Employees with shorter tenure (e.g., less than 3 years) have higher attrition rates, suggesting challenges in employee retention during the early stages of employment. 
    - Actions: Implement onboarding programs, career development initiatives, and performance feedback mechanisms to enhance employee engagement and loyalty.
  
### [4] Salary and Job Role Analysis:

- Employees with lower salary hikes or in certain job roles (e.g., lab technicians, sales executives) demonstrate higher attrition rates, indicating potential dissatisfaction with compensation or job responsibilities. 
    - Actions: Conduct salary benchmarking studies, performance evaluations, and career progression planning to ensure competitive compensation and growth opportunities for employees, thereby reducing turnover.

### [5] Work-Life Balance and Job Satisfaction:

- Employees with moderate work-life balance ratings and lower job satisfaction levels exhibit higher attrition rates, suggesting dissatisfaction with work conditions or organizational culture. 
    - Actions: Implement work-life balance programs, employee wellness initiatives, and regular feedback mechanisms to address workplace stressors and improve job satisfaction, fostering a positive work environment and reducing turnover.

The analysis offers valuable insights into employee attrition dynamics. To address the issues the organization should prioritize initiatives aimed at improving employee wellness initiatives to improve work life balance, career development programs, flexible work arrangements, regular feedback mechanisms.
