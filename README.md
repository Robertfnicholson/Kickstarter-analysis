# Kickstarting with Excel

## Overview of Project

Louise asked me for assistance to understand how different fundraising campaigns performed in  <br>
relation to their launch dates and their funding goals. Louise provided data on prior fundraising  <br>
campaigns. She would like me to analyze the data and provide conclusions to assist with future  <br>
fundraising campaigns.</p>

### Purpose

Perform analysis of Kickstarter dataset from fundraising campaigns to find trends. This analysis will  <br>
include developing visualizations for campaign outcomes based on their launch dates and their funding  <br>
goals.  The analysis and conclusions seeks to improve success of future fundraising campaigns.</p>

## Analysis and Challenges

To get started I reviewed the data set including each field, its field type, and number of  <br>
campaigns. I made two fields from the “category and subcategory” field using the text to column <br>
function. Also, to make use of the launch date and the deadline date which were Unix timestamps, I had  <br>
to convert the data into a standard date format using formulas. See screenshot below.  <br>
<br>
![Screenshot_Unix_TS_to_std_date.png](https://github.com/Robertfnicholson/Kickstarter-analysis/blob/e75e5ea905fea4ce166c36b43dd01217c8fb2373/Screenshot_Unix_TS_to_std_date.png)  <br>

I also used pivot tables and pivot charts to manipulate and to view the data in a particular <br>
way. This included filtering and sorting the data. I also used the freeze panes function to improve  <br>
viewing of the data. I used conditional formatting to provide improved visual information for the reader.  <br>
Also, I used statistical measures including mean, median, standard deviation and interquartile range to  <br>
understand the data better and developed box plots to compare distributions of data.  </p>

### Analysis of Outcomes Based on Launch Date

In this analysis I developed a pivot table of the data and then filtered the data to show only theater  <br>
campaigns and filtering outcomes of just successful, failed and canceled campaigns and filtering out live  <br>
campaigns. I then built a line graph of the outcomes by month. See graph below.  

![Theater_Outcomes_vs_Launch.png](https://github.com/Robertfnicholson/Kickstarter-analysis/blob/e75e5ea905fea4ce166c36b43dd01217c8fb2373/Theater_Outcomes_vs_Launch.png).   </p>

### Analysis of Outcomes Based on Goals

In this analysis I developed a table using the countifs() function to show the counts of successful, failed  <br>
and canceled campaigns for given dollar amount ranges of campaign goals. I then added calculation  <br>
fields that provide the percentage outcome for each given dollar amount range of campaign goals.  <br>
Finally, I developed a line chart displaying each of the outcomes based on the dollar amount ranges for  <br>
the x axis and percentage on the y axis. See graph below.

![Outcomes_vs_Goals.png](https://github.com/Robertfnicholson/Kickstarter-analysis/blob/e75e5ea905fea4ce166c36b43dd01217c8fb2373/Outcomes_vs_Goals.png).  </p>

### Challenges and Difficulties Encountered

I encountered several challenges in developing the visualizations. Most notably, I missed the instruction  <br>
on filtering out “live” campaigns. I reread the instructions after viewing the pivot table graphic. Also, I  <br>
used initially the singular countif() function for developing the launch date table. Once I reviewed the  <br>
hint on using the function, I realized it was the plural countifs() function.  Finally, I had to learn how to   <br>
write my report using Markdown format. To do this, I downloaded Notepad++ and used the application to prepare  <br>
the report.  </p>

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

The results indicate that the months with the most successful campaigns were May, June and July with  <br>
111, 100 and 87 successful campaigns, respectively. The month with the lowest successful campaigns  <br>
was December with 37. The range from highest to lowest was 74 (111-37) and the average was 69.9.  <br>
The month with the most failed campaigns was May with 52 and the month with the lowest was  <br>
November with 31. The range from highest to lowest was 21 (52-31) and the average per month was 41.1  </p>

- What can you conclude about the Outcomes based on Goals?

The results indicate that the two highest percentage successful campaigns, 75.8% and 72.7%, had the  <br>
two lowest goal ranges of "less than $1,000" and "between $1,000 to $4,999," respectively. The average  <br>
successful campaign percentage was 66.3%. The two lowest percentage successful campaigns, 0.0% and  <br>
12.5%, had the two highest goal ranges of "between $45,000 and $49,999" and "greater than $50,000,"  <br>
respectively. The average failed campaign percentage was 33.7%. Also, there were no canceled  <br>
campaigns in this subset.  </p>

- What are some limitations of this dataset?

The data only includes years 2014 to early 2017, so it is limited in its timeframe and is now nearly five  <br>
years old.  </p> 

- What are some other possible tables and/or graphs that we could create?

Use a pie chart to show the count of failed campaigns and the corresponding ranges of pledges to goals  <br>
say under 20%, 20%-40%, 40-60%, 60-80%, and over 80%. Also, calculate the length of each campaign,  <br>
develop ranges for campaign lengths, and then calculate the percentage success for campaigns in those  <br>
respective length ranges.  </p>