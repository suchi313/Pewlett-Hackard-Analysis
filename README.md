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

From the analysis, it was found that there is an oustanding # of employees who currently at the retirement age AND holding majority of the SR level titles. Reference the below subset of the table for Unique Titles. 

![image](https://user-images.githubusercontent.com/102767530/181661969-69f564e9-9083-4ef0-9428-d6240eb02397.png)

### Mentorship Eligibility/Candidates

After conducting the initial analysis and finding that majority of the employees were retiring, Pwlett-Hackward requested us to create a table showcasing senior level employees that can qualify to be members of the Mentorship Program. This program would aid new employees in achieving milestones in their new respective role.
![image](https://user-images.githubusercontent.com/102767530/181662394-538bb322-ebd9-4b5d-a29f-667fa5b7eb01.png)



