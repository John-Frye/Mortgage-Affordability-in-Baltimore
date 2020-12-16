# Mortgage-Affordability-in-Baltimore
Mortgage affordability in Baltimore over time 

## Background
Gentrification, or the influx of affluent residents, [can increase a neighborhood's cost of living and drive previous, low income residents from their homes](https://www.cdc.gov/healthyplaces/healthtopics/gentrification.htm). While gentrification often carries a connotation of "outside" wealth displacing a community, there is little research on the effects of investment and wealth generation by a neighborhood's own residents and a similar pattern of displacement. This lack of research could present problems for the Opportunity Zone program, a federal development plan that provides support and investment for small businesses in low-income neighborhoods. An ingress of investment to small, locally owned businesses might increase a neighborhood's household income, but could it also heighten the risk of displacement? Data analysis must establish whether or not a correlation exists between a neighborhood's living costs and the amount of its small business investment. If such a correlation exists, then stakeholders enacting the Opportunity Zone program, like Baltimore City Government, must invest in corresponding schemes aimed at reducing low-income residents' living costs. 

## Business Question
Does small business investment decrease mortgage affordability and, if so, how can economic development plans like the Opportunity Zone program maintain affordable living costs while also pursuing a path of growth? 

## Data Sources and Definitions
[Mortgage Affordability](https://github.com/John-Frye/Mortgage-Affordability-in-Baltimore/blob/main/Affordability_Index_-_Mortgage%20(2).csv): the percent of home mortgages in a population tract that are affordable to residents.

[Small Business Investment](https://github.com/John-Frye/Mortgage-Affordability-in-Baltimore/blob/main/Total_Dollar_Amount_Invested_in_Small_Businesses_per_50_Businesses%20(1).csv): the total amount of money invested in small businesses per 50 businesses in a population tract .

## Data Analysis
### Data Question(s)
What is the correlation between mortgage affordability and small business investment? How have these variables increased or decreased over time in Baltimore? 

### Python Analysis
Prior to conducting a data analysis on Python, I cleaned the data for mortgage affordability and small business investment in excel. As our target neighborhoods in the final project are few in number, I wanted to use all of the available data on the two metrics in Baltimore in order to establish a clear correlation, if one existed. I compiled all of the data from both variables and arranged it in a spreadsheet, with each value categorized by year (ranging from 2016-2018). 

I then uploaded this dataset to Python and averaged the values of each variable per year. Finally, I constructed a dual axis graph on Plotly that modeled how each variable changed over time in Baltimore. 

Insert Graph

From 2016 to 2018, mortgage affordability in Baltimore decreased on average. Conversely, small business investment increased during this time period. 

### Excel Analysis 
The relationship between mortgage affordability and small business investment is not circumstantial. Using excel, I calculated a correlation of -0.27 between mortgage affordability and small business investment. The correlation is negative, meaning that, as small business investment increases, mortgage affordability decreases. I checked that this correlation was statistically significant by performing a regression on the two variables. Small business investment's p value of 0.0076 is statistically significant, as it is below the statistically significant benchmark of 0.05. 

## Application to Final Project 
Given these findings, it appears that, in Baltimore, an increase in small business investment is likely to drive up the costs of living. It is possible that a corresponding increase in incomes from local businesses could offset this rise in living costs. However, to ensure that low-income residents are not displaced from designated Opportunity Zone neighborhoods, The Baltimore Department of Housing and Community Development should also invest in different housing programs designed to keep living costs affordable to low-income residents. This insight feeds into our final project's recommendation of three housing program components. 

Firstly, we recommend that the Department of Housing and Community Development should refurbish and transfer abandoned properties it already owns in target areas (described in the final report) to [community land trusts](https://www.bloomberg.com/news/articles/2019-04-29/alternative-homeownership-land-trusts-and-co-ops). For reference, community land trusts are non-profit corporations controlled by a neighborhood board that lease or sell properties at a low cost to low-income individuals. This strategy would provide a ready source of affordable housing to target areas' lowest income and most vulnerable residents.

For residents the majority of low-income residents (i.e. those not in poverty), we recommend that the Department of Housing and Community Development should increase funding for pre-existing housing voucher programs, which would mitigate rising housing costs without [distorting the overall market or limiting the ownership of an appreciating asset like a house](https://eicca.org/section-8). This latter strategy will play an increasing role over time, as the refurbishing of abandoned houses will likely [increase surrounding property's taxes and values](https://www.wichita.edu/academics/fairmount_college_of_liberal_arts_and_sciences/hugowall/documents/Topeka-Abandoned-Housing-Report-Final.pdf). 

## Additional Data
Additional data on what types of small businesses yield the highest decrease in mortgage affordability would be beneficial. This data could help inform the Department of Housing and Community Development of what types of small business it could target investment towards without significantly increasing the risk of displacement. Further research on the average increases in neighborhood income by small business type could provide additional context to this targeted funding decision. 

## Step by Step Instructions
Step by step instructions for how I completed the Python analysis can be accessed [via my Google Collaboratory](https://colab.research.google.com/drive/14BCsiCjGjfqA9FMcVNRgu-9R5d0WUtMw?usp=sharing).
Instructions for the excel analysis [can be found here](https://github.com/John-Frye/Mortgage-Affordability-in-Baltimore/blob/main/Mortgage_Affordability_Instructions.xlsx).
