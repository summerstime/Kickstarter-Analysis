# Kickstarter Analysis

## Overview of the Project

This project is to satisfy Challenge #1 in the Data Analytics Bootcamp. 
The client for this project is Louise, who wants to analyze various Kickstarter Project Campaigns and review campaign outcomes (success/failure, for example).  

### Purpose

The purpose of the analysis of the Kickstarter Campaign data is to provide Louise with needed information and visualization so that she can determine if she wants 
to move forward with her own campaign. It will also provide her direction on the type of campaign, goal setting, and time of year for her campaign to be successful.

## Analysis and Challenges

The analysis included the following items performed on the Excel data [Kickstart-Analysis](https://github.com/summerstime/Kickstarter-Analysis/blob/main/kickstarter_challenge.xlsx):
* Creation of additional columns for the Percentage Funded, Average Donation, Parent Category, Subcategory, Date Created Conversion, Date Ended Conversion, and Years.
* Conditional formatting was utilized on the Outcomes and Pledged columns. This helped distinguish the successes from the failures more easily in the spreadsheet.
* The original date columns were received in a UNIX Timestamp format and had to be converted using this type of formula =(((J2/60)/60)/24)+DATE(1970,1,1). 
* Equations, such as COUNTIFS(), AVERAGE(), and SUM(), were utilized.
* Pivot tables and charts were utilized to aggregate the data and allow for visualization in chart form. For the analysis discuss below, line charts were used. 

Challenges for this project include the following:
* Conversion of the UNIX Timestamp format to a recognizable month/day/year format. [UNIX Formula](https://www.extendoffice.com/documents/excel/2473-excel-timestamp-to-date.html)
* Review of the different pivot tables and charts to display the data in a way that provides useful information.

### Analysis of Theater Outcomes Based on Launch Date

The line chart below (Theater Outcomes Based on Launch Date), displays the different outcomes, successful/failed/canceled, for the main category of Theaters over each month of a year, regardless of the year. 
Along the left axis is the quantity of campaigns and along the bottom axis is the month.
Starting with the most promising month, the data show that the month of May is the most successful month with a quantity of 111. 
However after the month of May, the trend is downward in the number of successful campaigns and by December has reached the smallest quantity of all months at 37.
The quantities shift upward for both January and February with February reaching 71. 
A dip down in March equal to January's value of 56, turns around in April and May with successful and failed campaigns showing a maximum of 111 and 52, respectively.
Campaigns that have been canceled appear to be consistent across the year with January having the most at a quantity of 7.
In this display, there is no month where failed campaigns exceed in number beyond successful quantities. However the month of December has the closest numbers with 37 successful and 35 failed.

![Theater Outcomes Based on Launch Date](https://github.com/summerstime/Kickstarter-Analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png))

### Analysis of Outcomes Based on Goals

The line chart below (Outcomes vs Goals), displays the outcomes, successful/failed/canceled, of the subcategory Plays against the dollar amounts for each play's goal.
In this analysis of Plays, there were no data points for canceled plays. So the percentage results of successful and failed total to 100% for each goal increment.
Along the left axis is the percentage of successful/failed plays and along the bottom axis are the different goals in $5000 increments.
Starting with the lowest goal value group, less than $1000, the percentage of successful campaigns is at its highest (75.81%) and the percentage of failed campaigns at its lowest (24.19%).
As the goal dollars increase to $29,999, the trend of successful campaigns decreases consistently to a low of 20%. As the successful campaigns decrease, the failed campaign percentages increase to 80%.
Between $25,000 to $44,999, plays are successful again at about 66%. Moving beyond that dollar mount there is a much lower success rate from 0 to 20%.
  
![Outcomes vs Goals](https://github.com/summerstime/Kickstarter-Analysis/blob/main/Resources/Outcomes_vs_Goals.png))

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
  -Hosting Theater campaigns in May and part of the summer appears to be the best time of year.
  -Avoid hosting campaigns in the 4th quarter, less success, could be due to the holiday season.

- What can you conclude about the Outcomes based on Goals?
  -The lower campaign goals, less then $15,000, appear to be successful more often.

- What are some limitations of this dataset?
  -Comparison of different countries is difficult since the data set appears to be incomplete since it is heavily weighted to the US. 

- What are some other possible tables and/or graphs that we could create?
  -A graph for the number of Theater backers per launch month would provide information about which month typically has the most support.
  -A graph of the average donation of Theater per launch month provides a better understanding of the backer's support level. 
![Theater Backers](https://github.com/summerstime/Kickstarter-Analysis/blob/main/Resources/Theater_Backers_Launch.png)
![Average Donation](https://github.com/summerstime/Kickstarter-Analysis/blob/main/Resources/Ave_Donation_Theater_Launch.png)

