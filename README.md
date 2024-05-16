# cyclistic_capstone
Google Data Analystics Professional Certificate- Capstone project

## Scenario
The course simulates you working at a fictitious company, as the course briefing cites:

You are a junior data analyst working in the marketing analyst team at Cyclistic, a bike-share company in Chicago. The director of marketing believes the company’s future success depends on maximizing the number of annual memberships. Therefore, your team wants to understand how casual riders and annual members use Cyclistic bikes differently. From these insights, your team will design a new marketing strategy to convert casual riders into annual members. But first, Cyclistic executives must approve your recommendations, so they must be backed up with compelling data insights and professional data visualizations.

### Ask Phase
## Business task
The company's director of marketing wants to identify how do annual members and casual riders use Cyclistic bikes differently, with this, we can postulate a hypothesis about differences in user behaviour between casual riders and annual members. Hopefully, the results will culminate in getting more casual riders assigning for annual memberships.

### Preperation
This case study uses Cyclistic's historical trip data (previous 12 months) to analyze and identify trends. The data has been made available by Motivate International Inc. under and open license. The data can be dowloaded here.

Data credibility
Data can be considered reliable, original, comprehensive, current and cited. Despite the fact that in the Cyclistic trip data license agreement any warranty of accuracy is disclaimed, it can be considered overall reliable as well, even though being a fictitious dataset. It therefore provides us with the information needed to complete the business task.

### Process Phase
Tools I have used in this project
MS SQL: I believe that combining all the 12 months of data in SQL will be better for productivity, since there were plenty of repeated patterns on all the datasets.
Tableau: Provides data visualization and easily demonstrates the insights to the stakeholders.

Manipulation and cleaning of data
A series of steps were made to convey the maximum efficieny possible while manipulating and cleaning data, I find that cleaning with SQL is more efficient since you can join all tables and just do one command, instead of cleaning each dataset separately, this amount of data would be too much for Excel to handle.

You can check all the queries done on SQL with attached file. You can also check all the succesful changes that were made on the data set by going to the Changelog section at the end of this notebook.

Downloaded the files.
Saved the Cyclistic trip data in .csv and .xlsx format.
I used Excel to prepare data, checking if the data is reliable, original, comprehensive, current, cited and doesn't contain bias. Also used it to check what cleaning will have to be done on SQL.
Imported all data do MS SQL, joined all Cyclistic trip 12 months worth of data into a single file.
The following steps were taken in order to check data accuracy:
a. Ensured data format is correct: Data was imported in the correct format to MS SQL in order to be manipulated through SQL.
b. Checked and deleted null values: WHERE start_station_name, and end_station_name IS NULL.
c. Checked and deleted further inaccuracies, like 'ended_at' date earlier than 'started_at'.
d. Checked and deleted records with 'test', 'Test', 'TEST' in either 'start_station_name' or 'end_station_name'.
e. Added and populated the columns weekday and ride_length as shown in the changelog
f. Checked for spaces before and after string values.
g. Checked for misspellings in rideable_type and member_casual columns.
h. Checked for duplicates in ride_id.

### Analyzing the data
In this step, I analyzed the cleaned data to find out how annual members and casual riders use Cyclistic bikes differently.

You can check all the queries done on SQL in attached SQL file.
65% users are annual members whereas 35% are casual riders. We already have the majority of the customers signed for the annual membership.
In average, annual members use their bikes for 12 minutes and casuals used their bikes for 23 minutes.
Casual riders have by far the longest ride lengths. This is clear statement that casuals use their bikes sporadically.
Casuals have the biggest amount of rides on saturdays and sundays, but not for a wide margin.
Number of rides increases in an almost linear way throught the months, reaching its peak in summer months. Average ride duration tends to be the same all around the months.

### Share Phase
I created visualizations using tableau to communicate the results of my analysis. the dashboard can be found here https://public.tableau.com/app/profile/barsha.das/viz/Cyclistic_Case_Study_17152862278460/Dashboard2

We can see that although there are more annual members than casual riders, casuals represent a considerable percentage that can indeed increase Cyclistic’s revenue if they were to become annual members.

When I put the number of rides of casual and annual members in a week basis, it's possible to see that the amount of rides for the casuals increase considerably on weekends, but the number or rides for the annual members are higher on weekdays. Casual riders average ride duration is much higher than that of annual members. This point enables us to understand that bike usage is intrinsically different between annual members and casual riders.

We can formulate the initial hypothesis that casual riders use Cyclistic’s service for leisure purposes whereas annual members use it for shorter rides, like commuting to work.


### Act Phase
Steps for the future
Here are some insights to the marketing team aiming to answer the business task: Design marketing strategies aimed at converting casual riders into annual members.

Launch marketing campaigns in March or April, this is the period of the year when bike usage is greatly increased.
Social media ads targeting people who have already experienced any bike-sharing service and who are interested in travel, outdoor sports, parks, museum, Chicago touristic landmarks, etc.
Progressive discount on rates based on the ride length. The more minutes the members use the bikes the less they pay.



