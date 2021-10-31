# Kickstarting with Excel

## Overview of Project
My client, Louise wants to start her own Kickstarter campaign for her play, _Fever_, but is undoubtly unsure of her current set budget. In an effort to have a successful campaign, I was asked to analyze a dataset from Kickstarter's website to uncover trends about different campaigns.

### Purpose
The analysis was performed to help Louise set up her current crowdfunding campaign to be successful and help her plan future play projects.

## Analysis and Challenges
Initally, my analysis began on all Kickstarter campaings within the dataset by summarizing the data to understand the bigger picture. In the process, I used filters, conditional formatting, and PivotTables to understand what I was working with. Once my initial exploratory analysis was complete, I focused on the parent category of "theater" campaigns and the subcategory of "plays" campaigns.

### Analysis of Outcomes Based on Launch Date
To see how theater campaigns performed in general compared to when the campaigns started, I created a PivotTable based on the data from the "Kickstarter" sheet. To populate the PivotChart fields, parent category and years were added to filters field. I selected outcomes for columns, Date Created Conversion for rows, and count of outcomes for values. I removed the additional generated fields of "Years" and "Quarters" when selecting "Date Created Conversion" to leave months of the year as the x-axis. Then, I sorted outcome values in descending order. Lastly, I filtered outcomes to exclude live campaigns or campaigns still in progress leaving campaigns that were either successful, that failed, or were canceled. 

![PivotTable1](https://user-images.githubusercontent.com/91519293/139596602-b09d4481-fdfe-464c-ab20-67fe408b3e79.png)

Once the PivotTable fields were set up properly, I filtered parent category to show only theater campaigns. Below is the final PivotTable showing the different outcomes of theater campaigns by the month.

![PivotTable2](https://user-images.githubusercontent.com/91519293/139596745-ed680908-4ec1-4f48-a4c9-0778efaabf95.png)

From the PivotTable, I created a line chart to visualize the relationship between outcomes of theater campaigns vs launch month.

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/91519293/139597046-578a9a56-99be-49ac-8d1b-83e49bcc9db4.png)

### Analysis of Outcomes Based on Goals
Diving a bit deeper, I wanted to see the effect of proposed goal amount on play campaigns, if any. To get started, I filtered the "Kickstarter" sheet to only show campaigns under the subcategory: "plays". Following, I created a new sheet and added the following headers: Goal, Number Successful, Number Failed, Number Canceled, Total Projects, Percentage Successful, Percentage Failed, and Percentage Canceled. Under the "Goal" column, I created goal amount ranges so that projects could be grouped based on their goal amount. To fill in "Number Successful", "Number Failed", and "Number Canceled" columns, I used the COUNTIFS() function. In the column "Total Projects", each row is a summation of the values in "Number Successful", "Number Failed", and "Number Canceled" using the SUM() function. To determine percentages of successful projects, failed projects, and canceled projects, I took the respective number of projects divided by the total number of projects for the according goal range.

![Goal](https://user-images.githubusercontent.com/91519293/139602177-ba7f5abc-cab5-4e08-bb59-83afb048d743.png)

Once the table was completed and checked for errors, I created a line chart to visualize the the relationship between the outcomes of "plays" campaigns and goal ranges.

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/91519293/139602291-280528f7-8474-4f91-b0fc-5225f3f5e23a.png)


### Challenges and Difficulties Encountered


## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
