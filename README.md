# Kickstarting with Excel

## Overview of Project
With the conclusion of Louise's campaign for her play Fever she requested more information regarding other Theater campaigns and their success.  Based on the source data provided to us we analyzed various data points to provide a high level hypothesis on campaigns

## Analysis and Challenges

### Data Preparation
To begin the analysis we first transformed and simplified some of the data fields:
1. Added additional columns and formulas to better summarize the data as follows
   * Created Percentage Funded column `=ROUND(E2865/D2865*100,0)`
   * Created Average Donation column `=IFERROR(ROUND(E2865/L2865,2),0)`
   * Split Category and Subcategory into two columns by using text to column formatting
   * Converted Date Created and Date Ended from Unix to dates, `=(((J2865/60)/60)/24)+DATE(1970,1,1)`
   * Created Year column, `=YEAR(S2865)`
2. Became familiar with the data by creating pivot tables, charts and graphs

### Analysis of Outcomes Based on Launch Date
This analysis focused on all theater campaigns.  Based on launch date 25% of successful campaigns were launched in May and June.  Failed campaigns were relatively stable over the duration of this study running at an average of 41 per month.  Canceled campaigns were minimal at approximately 3% of all campaigns in the study.

![Outcomes Based on Launch Date](/katrina356/kickstarter-analysis/Resources/Theater_Outcomes_vs_Launch.png "Theater Outcomes")

### Analysis of Outcomes Based on Goals
This analysis focused primarily on plays within the Theater category.  Based on this analysis successful campaigns had goals that fell in the under $5K category or the $35K - $45K category.  However, 76% of successful campaigns had goals less than $5K while only 8% of successful campaigns had goals between the $35K - $45K goal. 

![Outcomes Versus Goals](/katrina356/kickstarter-analysis/Resources/Outcomes_vs_Goals.png "Outcomes vs Goals")

### Challenges and Difficulties Encountered
1. The data focuses solely on the goal set for funding and the launch date of the campaign.  Other factors may be contributing as to why a campaign succeeds or fails, such as:
   * The genre of the play such as comedy, romance etc.
   * Who is producing the play
2. At work I utilize a PC and excel thru and I am proficient in excel.  At home I've recently bought a MacBook Pro and working thru the differences in commands and processes has slowed down my progress.  

## Results

### Conclusions regarding Theater Outcomes based on Launch Date
- Campaigns have a better chance of succeeding if launched in May or June
- 60% of all campaigns are successful while 36% fail

### Conclusions regarding Outcomes based on Goals
- A campaign is more likely to succeed if the goal is under $5K

###Limitations to the dataset
- A majority of the data is from 2014 - 2016 prior years have minimal data points
- Not enough information.  As mentioned earlier there could be other reasons that the funding succeeded or failed as indicated in the statistics around the goals and pledges of successful and failed campaigns

###Other possible tables and/or graphs that we could create?
  * Duration of the Campaign.  Looking at the data set a majority of the campaigns were run in under 30 days
  * Descriptive statics around number of backers and average donation size may be helpful in determining if other factors may play into success or failure.  Successful campaigns on average have more backers and higher average donation size.  We need to look into why more people are donating to successful campaigns, what makes them so different

![Backers and Donation Size](Backers_and_Donation_Size.png)

