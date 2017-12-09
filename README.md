
This repository is for Final Project in Data 512 class. Please see file **a3_final_project_plan.ipynb** for project plan and file **d512_final_project_report.ipynb** for detailed code and report.

# Need of the day: People Analytics

## Abstract:

The goal of this project is to find a systematic pattern or trend (using employee data) and provide actionable insights towards enhancing employee retention. Following research questions are answered by applying data science techniques on employee data:
 * Question 1: Which employees are most likely to quit?
 * Question 2: What are the reasons for the employees to quit?
 * Question 3: How can a retention plan be created to enrich these employees?
The research successfully helped in exploring reasons on voluntary quits by employees. Using logistic regression on this dataset, we could predict employee attrition with an accuracy of ~76%. The probabilities calculated for each employee can be further used to enrich employees by providing personalized support and benefits. This is a win-win situation for both employer and employee. Significant findings from the research are summarized below:
* Satisfaction level of employees is the most important factor which determines employee turnover
* Employees promoted in last 5 years are more likely to stay
* Salary is not strongly correlated to attrition 
* Last evaluation for employees makes no difference in their decision to stay 

## Methodology
There are four major modules in this project. 
Following image depicts how these four modules interact with each other.
![alt text](https://github.com/dipsuw/data-512-final-project/blob/master/images/architecture.PNG)

## Data
Fields in the dataset(HR_comms_sep.csv) include:

Column name | Value | Description
--- | --- | ---
satisfaction_level | numeric | satisfaction level of each employee filled thru survey
last_evaluation | numeric | latest evaluation of an employee on a scale of 0 to 1
number_project | numeric | total number of projects employee has worked on
average_monthly_hours | numeric | average monthly hours worked by employee
time_spend_company | numeric | number of years employee has worked in a company
work_accident | numeric | binary value: 0 for work accident occured and 1 for no accident
promotion_last_5years | numeric | binary value: 0 for no promotion and 1 for promotion
salary | categorical | three categories of salary: high, medium and low(datatype changed to numeric)
sales | categorical | department of employee(name changed to department and datatype to numeric)
left | numeric | binary value: 0 for employee stayed and 1 for not stayed (name changed to attrition)

## License of the source data
This dataset is released under CC BY-SA 4.0, the details of this license can be found here(https://creativecommons.org/licenses/by-sa/4.0/)

## License for this project
* MIT License(https://opensource.org/licenses/MIT)

## Relevant documentation
* [1] Kaggle project https://www.kaggle.com/ludobenistant/hr-analytics
* [2] Latest report from Bureau of Labour https://www.bls.gov/news.release/jolts.nr0.htm
* [3] History of business intelligence https://www.betterbuys.com/bi/history-of-business-intelligence/
* [4] Article on solving attrition with data https://towardsdatascience.com/solving-staff-attrition-with-data-3f09af2694cd
* [5] Article on descriptive statistics https://www.marsja.se/pandas-python-descriptive-statistics/
* [6] Helpful linked in artcile on predicting employee attrition https://www.linkedin.com/pulse/predicting-employee-attrition-who-quit-when-praful-tickoo/
* [7] Helpful linked in artciles on predicting employee attrition https://www.linkedin.com/pulse/analyzing-employee-turnover-predictive-methods-richard-rosenow-pmp/
* [8] Use of Survival analysis for predicting attrition https://www.slideshare.net/twbriggs/survival-analysis-for-predicting-employee-turnover/24
* [9] Kaggle dataset https://www.kaggle.com/ludobenistant/hr-analytics/data
* [10]sklearn logistic regression http://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html
* [11]Logistic Regression example https://towardsdatascience.com/building-a-logistic-regression-in-python-step-by-step-becd4d56c9c8
* [12] Workforce analytics tool Visier https://www.visier.com/solutions/predict/
* [13] People analytics by Workday https://www.workday.com/en-us/applications/human-capital-management/people-analytics.html
* [14] Harvard Business Review article https://hbr.org/2017/06/hr-must-make-people-analytics-more-user-friendly
* [15] Categorical Encoding http://pbpython.com/categorical-encoding.html
* [16] Employee Attrition Risk Assessment paper http://rupeshkhare.com/wp-content/uploads/2013/12/Employee-Attrition-Risk-Assessment-using-Logistic-Regression-Analysis.pdfhttp://www.compensationforce.com/2017/04/2016-turnover-rates-by-industry.html
* [17] Turnover rates by industry http://www.compensationforce.com/2017/04/2016-turnover-rates-by-industry.html


## Attributions
* Link to the license for data https://creativecommons.org/licenses/by-sa/4.0/
* Changes to data: The values have not been changed in data. However there are few cosmetic changes made in data as follows:
    - 'sales' column name changed to 'department'
    - 'left' column name changed to 'attrition'
    - 'salary' column encoded to quantitative values [15]
    - 'department' column encoded to quantitative values [15]
    
