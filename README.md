# An Analysis of Kickstarter campaigns
Module 1 Challenge. Performing analysis on Kickstarter data to uncover funding trends
---

# Kickstarting with Excel
## Overview of Project
Two analyses of Kickstarter Campaign data were performed using the capabilities of Excel. Kickstarter Campaign data was organized, calculated, and analyzed to provide visualizations and comparison of funding Outcomes Based on Goals and Outcomes Based on Launch Date. Through this analysis it was observed that Play campaigns had the highest success rate when their goals were under $5,000, whereas higher goals of $45,000 and over had greater failure rates. In terms of launch dates, theater campaigns with launch dates between May and August had the highest success counts, however, theater had overall higher success counts overall compared to other categories. Live campaigns were deemed out of scope for this analysis as we are analyzing completed campaigns. 

### Purpose
The purpose of this project is to provide Louise with a comparison of different campaigns’ performance on Kickstarter in relation to their launch dates and funding goals. Trends in outcomes will be specifically observed for Theatre and Play campaigns.
## Analysis and Challenges
### Analysis of Outcomes Based on Launch Date
To evaluate the outcomes based on Launch Date, a pivot table was created using outcomes and launch dates from the Kickstarter data. Filters were added to further explore trends based on the Parent Category (Theater) and Years. Dates were grouped by month to provide a month over month comparison.  A Pivot chart was then produced from the pivot table to visualize the data. 
![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/81447450/112730412-65c2c500-8eff-11eb-9250-fee23752c6e7.png)


### Analysis of Outcomes Based on Goals
To evaluate the outcomes based on Goals, a new sheet was populated using the COUNTIFS() function to find Successful, Failed, and Canceled data based on dollar amount ranges for the fundraising goals in the Play subcategory. Using the newly populated data, Totals Projects were calculated in each row using the SUM() function. Percentages of successful, failed, and canceled projects were calculated using basic math functions to standardize the data. An “Outcomes Based on Goal” line chart was created to visualize the data using the dollar amount ranges and percentages of project outcomes.
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/81447450/112730419-73784a80-8eff-11eb-877d-b9bc3abe17da.png)


### Challenges and Difficulties Encountered
One of the biggest difficulties faced during the creation of Outcomes based on Goals was the number of manual calculations and long COUNTIFS() syntax. Due to the different dollar ranges and outcome categories, every cell had to be calculated differently with multiple COUNTIFS() ranges and criteria. This allowed for entry and calculation errors, requiring data to be double-checked. One way to check the data is to filter through the Kickstarter Data by the respective outcome, dollar ranges and subcategory and count how many rows are displayed. A quicker alternative is to use a pivot table to automatically count the sum of values. We could reuse our pivot table created for Subcategories and compare the sums for succesful, failed, and canceled projects.
![COUNTIFS_example](https://user-images.githubusercontent.com/81447450/112730499-e8e41b00-8eff-11eb-89a7-63efae03399f.png)
![Pivot_SubCategories](https://user-images.githubusercontent.com/81447450/112732800-1afa7a80-8f0a-11eb-9b04-7f22a3e8fd9f.png)


## Results
#### What can you conclude about the Outcomes based on Goals?
The data shows that Play campaigns with goals under $5,000 had the highest success rates, the highest success for campaigns with goals less than $1000 with 76% successful projects.
<img width="770" alt="Outcomes_vs_Goals_chart" src="https://user-images.githubusercontent.com/81447450/112730486-d4a01e00-8eff-11eb-98fa-34a1e3e6795e.png">

In contrast, goals of $45,000 and over had greater failure rates. The highest failure rates for campaigns occurred for those with goals between $45,000 and $49,999 with 100% failed projects. In the Outcomes Based on Goal chart, we can see that after $1500, percentages of successful and failed campaigns fluctuate more. Overall, it can be concluded that lower funding campaign goals have a higher success than those with higher goals. 

#### What are two conclusions you can draw about the Outcomes based on Launch Date?
Theater campaigns with launch dates between May and July had the highest success counts. The highest being in May with 111 successful Theatre campaigns, compared to 37 successful campaigns in December. Overall successful campaigns are highest in the middle of the year and dip towards the end of the year. 

Another observation is that very few Theatre campaigns are canceled regardless of launch date. While failed campaigns are consistent throughout the year, there are significantly higher successful Theatre campaigns. However, theater had overall higher success counts overall compared to other categories. This could mean that Theatre has a large support base. 
![Parent_Category_Outcomes_allcountries](https://user-images.githubusercontent.com/81447450/112730533-14670580-8f00-11eb-9588-df25523477ae.png)

#### What are some limitations of this dataset?
A limitation of the Kickstarted Data set is that outliers are not identified. The goals dollar amounts are between $1.00 and $100,000,000, which is a big range and both dollar amounts are unrealistic for campaign goals. Identifying outliers that may be skewing the data could help provide a better picture of the outcomes. 
Another limitation is that we do not know if the outcomes were solely due to the dollar goal or the launch date; there are external factors that the data set does not account for. It would be useful to know the reason for canceled and failed outcomes.

#### What are some other possible tables and/or graphs that we could create?
It is recommended to perform a deeper analysis of successful Plays to further investigate factors of success: 
* Creating a bar chart for Backers vs Pledged will allow us to understand donor contribution. 
* We could also analyze success data based on country by creating a Country vs Outcomes bar chart to see if success differs outside the US. 
* Lastly, to dig further into the launch dates we could compare length of campaigns to see if overall campaign duration affects outcomes. We would need to calculate campaign duration in days and create a line graph depicting percentage of successful, failed, canceled campaigns.

