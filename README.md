# Kickstarting with Excel

## Overview of Project
	Gathering and analyzing data from the outcome of theater plays based on their launch date and their over funding goal.
### Purpose
	The purpose of this project was to find information for client on how different kickstarter campaigns had fared in relation to their launch dates and their funding goals. The client had their play's fundraising goal nearly acheived in a short amout of time so, she wants to know about other compaigns outcomes by using the goal and launch date criteria.
	
## Analysis and Challenges
	To anlayze the data from theater outcomes by launch date we created a pivot table that filters by the Parent Category of the Kickstarter campaigns and by the year they occured. Columns are divided by the outcomes, Rows are divided by the Month the Kickstarter began, and the values in the table are counting the number of outcomes for each criteria. 

	![Theater_Outcomes_by_Launch_Date_Table](https://user-images.githubusercontent.com/78178900/110382958-41bb4480-8021-11eb-93c1-6458979b855e.png)

	With this table we can see the total number of successful, failed, and canceled outcomes from each kickstarter that was in the Theater category. We can also see the total number by each month for each outcome to see which month is the best and which is the worst for starting a campaign. May has the most successful campaigns and December has the least, May also has the most failed campaigns and November has the least. We used the data from the table to create a chart to easily look at the change in trends. The chart is located below under *Analysis of Outcomes Based on Launch Date*

	To analyze the data from theater outcomes by goals we created a table that shows the number of successful, failed, and canceled campaigns (labeled Total Projects instead of campaigns) based on the amount that the campaign had set a goal for. 

	![Outcomes_Based_on_Goals_Table](https://user-images.githubusercontent.com/78178900/110382978-497ae900-8021-11eb-92b8-c5ae97fef4f6.png)

	We split the goals into separate ranges so we can look closer at the success rate based on the dollar amount set as a goal. We then calculated the successful, failed, and canceled rate by percentage. The highest rate of success based on percentage for any of the ranges is 76%. We then used the data from the table to create a line chart so we can easily see the change in trends for this data set. The line chart is located below under *Analysis of Outcomes Based on Goals*

	Some challenges that arise when analysing this data is that there is a lack of data points among certain criteria; for example, there are 534 total campaigns that had a funding goal range of $1000 to $4,999. There is a total of 1 campaign that had a funding goal range of $45,000 to $49,999. This can present a challenge because having 534 data points may allow you to find some clear probability of outcomes but having only 1 is not enough to truly understand the probablility of outcome for that particular funding range. If we had the same amount of data points among both criteria it would allow for much better analysis of the campaign outcome.

	Another challenge was that the data from the Theater Outcomes by Launch Date was not filtered by the subcategory for "plays" and the Outcomes Based on Goal data were filtered by that subcategory. This makes it challenging to see the true relation between the two data sets.

### Analysis of Outcomes Based on Launch Date
![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/78178900/110383090-6f07f280-8021-11eb-9c12-ff741941c1ae.png)

	Based on the analysis of launch dates there is a clear trend of May being the month with the highest rate of success. It is also the highest month for failures; on the other hand, it also has the largest difference between number of failed and number of successful campaigns with 111 successful and 52 failed. The months May, June, and July have the highest success rates which could be used as a good indication that these months are the best to choose when launching a kickstarter campaign.

### Analysis of Outcomes Based on Goals
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/78178900/110383004-54ce1480-8021-11eb-8e5b-97257ceac8ae.png)

	Based on the analysis of funding goals you can see that the range with the highest percentage of success is a funding goal that is less than $1,000 with a success rate of 76%. The range with the second highest percentage rate of success is a funding range between $1,000 to $4,999 with a success rate of 73%. When looking at the percentages it is clear which has a higher rate of success however I believe it is noteworthy to point out that the total number of campaigns that had a funding goal of less than $1,000 is 186. The total number of campaigns with a funding goal between $1,000 to $4,999 is 534. It would appear that choosing less than a $1,000 for a goal would achieve the most success but since it has a much smaller data set it may be that between $1,000 to $4,999 is the best range to choose. Nonetheless, according to the data as long as your funding goal is less than $5,000 then you will maximize your probability of achieving your campaign funding goal.

### Challenges and Difficulties Encountered

	Challenges that were encountered were the lack of constistency in the number of data points among the different criteria. Percentages can be very deceiving because if you have one row of your data set with a large total amount of data points and another row with a very low number of data points you may end up with similar percentages or largley differing percentages which, can give false represntations of potential outcomes. For example, the funding goal range of $45,000 to $49,999 has a failure rate of %100 and the range of $40,000 to $44,999 has a failure rate of %33 but both ranges have a total number of 1 failed campaign. This can be highly misleading and become a challenge when using the data to influence effective decision making.

	When referring to the analysis process some difficulties were encountered when creating formulas for the outcomes based on goals. Using certain functions can be tricky especially when you're creating longer functions and if you are missing quotations where needed or an apostrophe then your function will return an error. Be sure to always double check for any missing punctuation in your formulas to ensure they operate correctly with no errors. 

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
	
  - Two conclustions that you can draw are that May is the best month to launch your kickstarter campaign for plays, and that December is the worst month to start it. This is because May has the highest amount of successful campaigns. December has the least amount of successful campaigns which, are almost equal to the amount of its failed campaigns.

- What can you conclude about the Outcomes based on Goals?

  - We can conclude that having a total funding goal that is less than $5,000 will maximize your probability of achieving your goal. This is because the two funding ranges below $5,000 have the two highest success rates. We can also conclude that we need more data points in the ranges that are above $15,000 to make a solid conclusion of the outcomes and how they fare. 

- What are some limitations of this dataset?

  - Some of the limitations include the following:
	1. We don't see the outcomes based on goals and the months that they were launched. 
	2. We don't see the country that these campaigns were created in.
	3. The data set for outcomes based on launch date are only filtered by parent category and not the subcategory for plays.

  - A limitation in the Kickstarter sheet is that we can only see the average amount of each backer. If we could see how much each individual donation was for each individual campaign then we could find if there are any outliers that are skewing the average donation. This could also give us a better look into how many backers are outliers for each campaign and which campaigns would have failed if they did not include those outlier backers. Removing the outliers could affect the success/failure rate and reveal different conclusions. In addition, we could calulate the probability of there being an outlier backer in your campaign which can manipulate how we interpret the data. 

- What are some other possible tables and/or graphs that we could create?
	
	- We could create a table that shows the Outcome Based on Launch Date with the subcategory filter set to "plays" and then we could use that table to creat another pivot chart similar to the one with the parent category filter in place.

	- We can also add the Country filter to both the table and chart so that we can filter by country to see the outcomes based on launch date for campaigns in the US. 

	- Another chart and table can be made to see the amount of successful, failed, and canceled campaigns based on Launch Date and of a specific Funding Goal range in the US by each year and month. This could allow us to see any positive change in trends that could give indications of growing or declining popularity in certain parent and subcatgories and can give us a deeper look for analysis.
