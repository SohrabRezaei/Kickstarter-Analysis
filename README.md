# Kickstarter-Analysis

## Overview of Project

Louise has asked us to analyze various fundraisings to understand better the factors involved in launching a campaign for herself.

### Purpose

After going over multiple factors related to launching the campaign, she has decided to emphasize finding the relationship between the aftermath of these campaigns based on the month they were established and the amount of money they were supposed to attain.

## Analysis and Challenges

Since there are two different projects, we basically break down the analyses into two sections and discuess their challenges.

### Analysis of Outcomes Based on Launch Date

In the new KickStarter_Challenge worksheet, we have created a new column named Years. The values of the column are extracted from the date created conversion column by using [Year()](https://support.microsoft.com/en-us/office/year-function-c64f017a-1354-490d-981f-578e8ec8d3b9) ![Year screenshot](year.PNG).

Then I created a pivot table and named the new sheet 'Theater Outcomes by Launch Date'. I put the Parent Category and Years in the filter section; date created conversion in the rows sections, and outcomes in both the column and values section. I removed the years and quarters field from the rows sections to show only months in my pivot table. I changed the Parent Category filter to Theater only, and by clicking the column labels section, I managed to filter the life and blank out of my dataset. I also used descending order to show the successful outcome in the first column. Finally, I inserted a line with markers chart and chose a suitable title to demonstrate my project
[![Theater-Outcomes-by-Launch-date.jpg](https://i.postimg.cc/YSWHZKST/Theater-Outcomes-by-Launch-date.jpg)](https://postimg.cc/d7wpZfr9)

### Analysis of Outcomes Based on Goals

First I created Goal, Number Successful, Number Failed, Number Canceled, Total Projects, Percentage Successful, Percentage Failed and Percentage Canceled columns. Then, [Countifs()](https://support.microsoft.com/en-us/office/countifs-function-dda3dc6e-f74e-4aee-88bc-aa8c2a866842?ui=en-us&rs=en-us&ad=us) was used by filtering the outcome,the goal's range that each campaign fall under and "plays" subcategory.[![outcomes-based-on-goals.jpg](https://i.postimg.cc/YSp6yk8C/outcomes-based-on-goals.jpg)](https://postimg.cc/mP51tv0v)
[Sum()](https://support.microsoft.com/en-us/office/sum-function-043e1c7d-7726-4e80-8f32-07b23e057f89) was key in calculating the total projects. Finally, each outcome was divided by total projects and converted to percentage in order to calculate the percentage of successful, failed and canceled projects. Finally, a line chart presented the relationship between outcomes and the desired goal ranges.

### Challenges and Difficulties Encountered

If we wouldn't create the year's column in the first place, we could not filter it based on years in the pivot table. Displaying months for the pivot tables was a bit challenging to figure out by removing the years and quarters in the rows section of the pivot table. Utilizing the countifs function was time consuming since it had three arguments in this specific case, and we must use $ before the column names in order to use this formula multiple times by dragging the cell.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

1.May is the busiest month in both successful and failed projects and Summer being the busiest month in successful projects.

2.Both successful and failed projects display a similar trend throughout the year.

- What can you conclude about the Outcomes based on Goals?

The goal range of 1000-5000 has the highest number of successful projects. There weren't any canceled projects in our dataset.

- What are some limitations of this dataset?

The goal range of 35000-45000 has high percentages of a successful project, but the sample size of its total projects is minimal, making us second guess our whole analysis. In general, the sample size of total projects is not even throughout the entire range, so talking about percentages is somewhat biased.


- What are some other possible tables and/or graphs that we could create?

One possible table that could have been created may be the outcome of these campaigns based on the time that it takes to reach the goals for the successful ones. Bar chart could be utilized for the outcomes based on goal, since there is no time factor involved in it.
