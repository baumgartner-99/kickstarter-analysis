# Kickstarting with Excel
## Overview of Project

### Purpose

The purpose of this analysis of the Kickstarter dataset is to understand the outcomes of different campaigns based on their launch dates and funding goals. For this analysis, we specifically look at campaigns for funding theater projects, such as plays. 

## Analysis and Challenges

I created two visualizations to analyze outcomes based on two different criterion: launch date and funding goal. 

### Analysis of Outcomes Based on Launch Date

![Theater Outcomes vs Launch](https://github.com/baumgartner-99/kickstarter-analysis/blob/main/Theater_Outcomes_vs_Launch.png)

To create a visualization of theater outcomes based on launch date, I created a pivot table in Excel and filtered values with the parent category, theater. This graph shows the number of campaigns launched during different months of the year. Each line represents a different outcome: blue - successful, orange - failed, and gray - canceled. 

### Analysis of Outcomes Based on Goals

![Outcomes vs Goals](https://github.com/baumgartner-99/kickstarter-analysis/blob/main/Outcomes_vs_Goals.png)

To create a visualization showing outcomes of campaigns based on funding goal, I created a new table with the rows representing different ranges of financial amounts in US dollars. I then took counts of campaigns in each outcome per dollar amount range. Finally, I calculated the percentage of campaigns in each outcome by the total projects with a funding goal in that respective range. On the chart, the blue line represents the percentage of successful campaigns with various funding goals; the orange line represents percentage of failed campaigns; and finally, the gray line is the canceled campaigns. 

### Challenges and Difficulties Encountered

One particular challenge I ran into while analyzing this dataset was with the outcomes based on goals portion. While finding the count of each campaign outcome, I at first forgot to include "equal to" operators on the ranges of financial goals. For instance, my first line chart showed only values that were greater than 1000 and not equal to 1000 or less than 50000 and not equal to 50000, etc. This threw off my entire line chart, as I was missing a few important values. Luckily, I caught the error before saving the chart and was able to adjust my formulas accordingly. 

I did not encounter any challenges in my analysis with the outcomes by launch date, but I suspect the chart may have been difficult to form if the launch dates were not formatted properly. For instance, the chart would look totally different if one had created the pivot table rows to be arranged by year of launch instead of month. That would have been difficult to visualize with a single line chart. 

## Results

Conclusions can be made about the chart representing Theater Outcomes by Launch Date. For instance, most successful campaigns were launched during the month of May with a steady decline with campaigns launched later in the year. On the other hand, failed campaigns were relatively unaffected by the month they were launched. Of course, there is some change with October and May being peak months at about 50 campaigns and the lowest being November and March at about 30 campaigns.

Regarding Outcomes Based on Goals, it is interesting to note that there were no canceled campaigns that were plays. The percentage is zero across all ranges. Furthermore, there does not seem to be any significant relationship between funding goals and the outcome of the campaign. The two outcomes of course an inverse relationship with each other. 

Some limitations of this dataset are that it doesn't include any data on marketing or fundraising techniques. That is another factor that can influence campaign outcome as successful or failed. Furthermore, it includes campaigns that are live which can skew data if it is not filtered out. 

Another table that may be useful for this type of analysis is to further categorize the plays by genre to see if any specific genre is more popular than another. We could also zoom in on the successful campaigns and create a timeline to see if the number of campaigns grew over time. That could serve as an initial assessment if fundraising techniques are working or progressing to achieve a successful result.
