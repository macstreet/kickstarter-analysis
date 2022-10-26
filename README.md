# Kickstarting with Excel

## Overview of Project

### Purpose

  The purpose of this analysis was to review outcomes of theater kickstarters in two different ways. First, outcomes were broken out by the month the kickstarter was launched. The second angle of analysis was reviewing outcomes based on the funding goals of the kickstarter. 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

- Overview of Analysis

  This analysis was performed by creating a pivot table which was filtered by Parent Category (Theater) and Year. In the columns were outcomes, rows were Launch Date month (referred to as Date Created Conversion) and values were the number of outcomes. A line chart was then created with each line representing the number of successful, failed, and canceled theater kickstarters across the month of their launch date. 


![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/114192448/197914950-db2784f8-5f51-412d-b8fd-06b3ccacf802.png)



### Analysis of Outcomes Based on Goals

  This analysis was performed by starting with a table that broke down ranges of funding goals. In order to obtain the number of kickstarter projects within each range, I used the COUNTIFS function, and entered the critera for that goal range, outcome, and subcategory (play). For each criteria within the formula, I referenced the sheet Kickstarter sheet using an exclamation point, then the column range, then the value of what I wanted counted in that column. I made sure that the $ was entered with the column ranges so the ranges would remain constant and I could copy the formula across the table and only need to edit small sections of the formula to meet the criteria of what that cell. I then used the SUM function to find the total of each outcome of projects, as well as the total number of projects in each goal range. In order to find the percentage of each outcome and goal range, I divided the number of projects with a certain outcome by the total project. I then formatted these cells into percentages.

  I then created a visual representation of the percentage of outcomes into a line chart, with each line representing a outcome across the goal ranges. 


![Outcomes_vs_Goals](https://user-images.githubusercontent.com/114192448/197914878-f945b2ba-4434-4084-bacb-82f4e3ba1e60.png)


### Challenges and Difficulties Encountered

I had some difficulty with constructing the pivot table at first - particularly with figuring out how to break the Date Created Conversion in the row into months rather than quarters or years. In the end I figured out that I was simply overthinking it, and all I needed to do was delete the two fields I didn't want, and I was left with the row broken out into months. 

I also found completing the table of COUNTIFS formulas quite challenging. It wasn't for a lack of understanding, I found myself needing to check and recheck that I did not mistype anything or forget to add a criteria. The first mistake that I made when creating the table was neglecting to use the constant $ which made copying the formula accurately impossible at first. Then I realized I had made an error with typing in the number ranges, missing a "9" here and there. My typos made me extra cautious to the easy errors I could make, and how I needed to be checking my work regularly. When the number of canceled plays all came up as zeros, I once again, thought I had made an error. I checked and rechecked my formula, and then I decided to go back to my dataset, and filter for plays that had been canceled. Of course there were zero, therefore confirming that I was not incorrect. 

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

  Based on the line chart, the significant spike in successful outcomes would suggest that the month of May, and the summer months overall would be the best time to launch a kickstarter theater project.
It would also appear that December would be the riskiest time to start a kickstarter theater project, as historically the success rate seems to be 50%. 

- What can you conclude about the Outcomes based on Goals?

  The most of the successful plays appear to have a goals less than $4,999. The only other time kickstarters were more successful than failures were the plays that had goals between $35,000 and $44,999. Kickstarters with goals higher than $45,000 were almost always likely to fail.

- What are some limitations of this dataset?

  The limitation of Outcomes by Launch Date analysis is the lack of percentage data. The pivot table only gives final numbers of success, failed, canceled and total - we can't necessarily take at a large number of successes during one month and deem that a high success month without taking into account the total number of projects launched during that month. A percentage of how many successes to failures to cancels over the overall total of projects launched can give a more standard evaluation across months. 

  A limitation of the Outcomes Based on Goals dataset is the focus on the subcategory of "plays." The Launch Date analysis focuses on the category of Theater kickstarters, and whereas Goals analysis zooms in on a tighter analysis of just Theater/Plays. If we are to get an accurate view across both analyses, we should be looking at the same parent category and subcategory for both.

- What are some other possible tables and/or graphs that we could create?

  A clustered bar chart could also demonstrate theater outcomes based on launch date in an understandable way.

![Outcomes by Launch Date Bar Chart](https://user-images.githubusercontent.com/114192448/197914995-c86d38b2-4865-471c-9a6e-601aec0bca3f.png)

