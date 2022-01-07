# Kickstarter-Analysis
## Overview of Project
Louise has asked us to analyze various fundraisings to understand better the factors involved in launching a campaign for herself.
### Purpose
After going over multiple factors related to launching the campaign, now she has decided to emphasize finding the relationship between the aftermath of these campaigns based on the month that they were established and the amount of money they were supposed to attain.
## Analysis and Challenges
Since there are two different projects, we basically breakdown the analyses into two sections.
### Analysis of Outcomes Based on Launch Date
In the new KickStarter_Challenge worksheet, we have created a new column named Years. The values of the column are extracted from the date created conversion column by using [Year Function Syntax](https://support.microsoft.com/en-us/office/year-function-c64f017a-1354-490d-981f-578e8ec8d3b9) ![Year screenshot](year.PNG).
Then I created a pivot table and named the new sheet 'Theater Outcomes by Launch Date'. I put the Parent Category and Years in the filter section; date created conversion in the rows sections, and outcomes in both the column and values section. I removed the years and quarters field from the rows sections to show only months in my pivot table. I changed the Parent Category filter to Theater only, and by clicking the column labels section, I managed to filter the life and blank out of my dataset. I also used descending order to show the successful outcome in the first column. Finally, I inserted a line with markers chart and chose a suitable title to demonstrate my project
[![Theater-Outcomes-by-Launch-date.jpg](https://i.postimg.cc/YSWHZKST/Theater-Outcomes-by-Launch-date.jpg)](https://postimg.cc/d7wpZfr9)
### Analysis of Outcomes Based on Goals
First I created Goal,Number Successful,Number Failed,Number Canceled,Total Projects,Percentage Successful,Percentage Failed and Percentage Canceled columns. Then, [Countifs function syntax](https://support.microsoft.com/en-us/office/countifs-function-dda3dc6e-f74e-4aee-88bc-aa8c2a866842?ui=en-us&rs=en-us&ad=us) was used by filtering the outcome,the goal's range that each campaign fall under and "plays" subcategory.[![outcomes-based-on-goals.jpg](https://i.postimg.cc/YSp6yk8C/outcomes-based-on-goals.jpg)](https://postimg.cc/mP51tv0v)
[Sum()](https://support.microsoft.com/en-us/office/sum-function-043e1c7d-7726-4e80-8f32-07b23e057f89) was key in calculating the total projects.



