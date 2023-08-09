# Employee Attrition Predictor

# 1. Introduction
- Employee attrition is when an employee leaves the company through any method, including voluntary resignations, layoffs, failure to return from a leave of absence, or even illness or death.
- High attrition rates for employees are often due to poor job satisfaction, an aging workforce, spending cuts, or increased competition.
- The direct impacts are relatively easy to measure: costs must be incurred to recruit and train new employees. During the recruitment process, other employees generally see an increase in their workload which can result overtime costs, but also affect their own productivity
- We’re going to create an algorithm for employee attrition prediction i.e. predicting that employee will leave the current company or will resign from the current company.

# Problem Statement

## Current Practice

- Once an employee leaves, he or she is taken an interview with the name “exit interview” and shares reasons for leaving. 
- The HR Department then tries and learns insights from the interview and makes changes accordingly.
<center> <img width=60% src="https://theinvestorsbook.com/wp-content/uploads/2019/10/Purpose-of-Exit-Interviews.jpg"> </center>

## This suffers from the following problems:

   1. This approach is that it's too haphazard. The quality of insight gained from an interview depends heavily on the            skill of the interviewer.
   2. The second problem is these insights can't be aggregated and interlaced across all employees who have left.
   3. The third is that it is too late by the time the proposed policy changes take effect.

# Our Objective
  
  - The HR Department at a software company want to try a new initiative to retain employees.
  - The idea is to use data to predict whether an employee is likely to leave.
  - Once these employees are identified, HR can be more proactive in reaching out to them before it's too late.
  - They only want to deal with the data that is related to permanent employees.
   
   <center> <img width=60% src="https://www.springml.com/wp-content/uploads/2020/08/employee-attrition.png"> </center>

The HR department has hired you as data science consultants. They want to supplement their exit interviews with a more proactive approach.


# Data Acquisition & Description
- The Business Intelligence Analysts of the Company provided you **three datasets** that contain information about past employees and their status (still employed or already left).
-  **3 tables** are as below...

**Table No. 1**

##### ***department_data***

This dataset contains information about each department. The schema of the dataset is as follows:

   1. **dept_id** – Unique Department Code
   2. **dept_name** – Name of the Department
   3. **dept_head** – Name of the Head of the Department

**Table No. 2**   

##### ***employee_details_data***

This dataset consists of **Employee ID, their Age, Gender and Marital Status**. The schema of this dataset is as follows:

   1. **employee_id** – Unique ID Number for each employee
   2. **age** – Age of the employee
   3. **gender** – Gender of the employee
   4. **marital_status** – Marital Status of the employee

**Table No. 3**
##### employee_data

This dataset consists of each employee’s **Administrative Information, Workload Information, Mutual Evaluation Information and Status**.

##### Target variable

   1. **status** – Current employment status (Employed / Left)
    
##### Administrative information

   1. **department** – Department to which the employees belong(ed) to
   2. **salary** – Salary level with respect to rest of their department
   3. **tenure** – Number of years at the company
   4. **recently_promoted** – Was the employee promoted in the last 3 years?
   5. **employee_id** – Unique ID Number for each employee
    
##### Workload information

   1. **n_projects** – Number of projects employee has worked on
   2. **avg_monthly_hrs** – Average number of hours worked per month
    
##### Mutual evaluation information

   1. **satisfaction** – Score for employee’s satisfaction with the company (higher is better)
   2. **last_evaluation** – Score for most recent evaluation of employee (higher is better)
   3. **filed_complaint** – Has the employee filed a formal complaint in the last 3 years?


