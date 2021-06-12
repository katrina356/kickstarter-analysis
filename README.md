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


### Analysis of Outcomes Based on Goals
This analysis focused primarily on plays within the Theater category.  Based on this analysis successful campaigns fell in the under $5K category or the $35K - $45K goal.  However, 76% of successful campaigns were less than $5K in goal while only 8% of successful campaigns were between the $35K - $45K goal. 

### Challenges and Difficulties Encountered
1. The data focuses solely on the goal set for funding and the launch date of the campaign.  Other factors may be contributing as to why a campaign succeeds or fails, such as:
   * The genre of the play such as comedy, romance etc.
   * Who is producing the play
2. 

## Results

### Conclusions regarding Outcomes based on Launch Date
- Campaigns have a better chance of succeeding if launched in May or June
- More campaigns are successful than fail

### Conclusions regarding Outcomes based on Goals
- A campaign is more likely to succeed if the goal is under $5K
- A campaign is more likely to fail if the goal is set between $25K and $35K

###Limitations to the dataset
- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
