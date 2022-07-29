# Pewlett-Hackard-Analysis

## Overview
The main objective of this analysis was review the data given to us by Pewlett Hackard, conduct a database analysis using PostGreSQL, and provide results that showcased the # of future retirees across all departments that are currently employeed. The results aided the company in preparing a gameplan to hire and onboard new employees but also look into a mentorship opportunities for the tenured employees to mentor the new employees. 

Overall, throughout the course of the challenge we had to create 4 tables. Mentorship_Elgibility, Retirement_Titles, Retiring_Titles, and Unique_Titles.
The criteria for identify the retired employees was based off their birthdays and dates hired. The dates for birthday ranged from 1952-1955 and hired dates from 1985-1988. 

## Resources 
- PostgreSQL + pgAdmin

## Results 

Before creating the analysis, we were tasked to create an Entity Relationship Diagram (ERD). This helped us identify and visualize the relationship between the various entities - being data sources and the variety of different structures the company had in place. 

![EmployeeDB](https://user-images.githubusercontent.com/102767530/181659203-36b5a9f7-d71a-4ef0-bbbb-893e7c5fe3e3.png)

### How Many Employees are in a Position to Retire
1. To identify how many employees were ready to retire - we first had to gather the employees born between Jan, 1st 1952 - Decemeber 31st, 1955. I did this by writing code in SQL that returned Employee Number (e.emp_no), First Name (e.first_name), Last Name, Title, From Date, and To Date of all the employees within the company that were born on the dates specified earlier. 
-  ![image](https://user-images.githubusercontent.com/102767530/181663667-50b38987-a77f-419c-bd56-5b71baa9e644.png)

2. To ensure we removed ALL duplicate records, I used the following code - 

  ![image](https://user-images.githubusercontent.com/102767530/181664119-bd6bb9f5-313c-4a0a-bbf7-ca87d4978ed6.png)
  
3. From the analysis, it was found that there is an oustanding # of employees who currently at the retirement age AND holding majority of the SR level titles. Reference the below subset of the table for Unique Titles. 

![image](https://user-images.githubusercontent.com/102767530/181661969-69f564e9-9083-4ef0-9428-d6240eb02397.png)


### Mentorship Eligibility/Candidates
After conducting the initial analysis and finding that majority of the employees were retiring, Pwlett-Hackward requested us to create a table showcasing senior level employees that can qualify to be members of the Mentorship Program. This program would aid new employees in achieving milestones in their new respective role.

The below query is similiar to the original one. The only difference is adjusting the birthdate - this allows to be inclusive of employeeds born in 65'.

![image](https://user-images.githubusercontent.com/102767530/181664524-34cfe4ff-21f8-4613-91f6-2ba229c920a2.png)

Below is the table for those eligbile to partake in the mentorship program. 

![image](https://user-images.githubusercontent.com/102767530/181662394-538bb322-ebd9-4b5d-a29f-667fa5b7eb01.png)

### Summary 

1. How many roles will need to be filled as the "silver tsunami" begins to make an impact?
2. Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?

