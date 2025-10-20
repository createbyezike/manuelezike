# manuelezike
Microsoft PowerBI
For this project, I was responsible for creating an interactive dashboard to track digital marketing campaign performance across Email, Instagram Ads, Influencer Marketing, and other channels. The goal was to provide the marketing team with actionable insights into spend efficiency, engagement, and ROI. This process required three stages:

1.Data Quality Assessment (assess the quality of data and make recommendations to clean the underlying data and mitigate the issues causing unclean data).

2.Data Insights (clean and explore the data, develop the model that can be used to target potential profitable customers and generate insights).

3.Data Presentation (develop an interactive dashboard to display data summary and results of the analysis).

DATA QUALITY ASSESSMENT
This stage involves examining the data to identify any issues or errors that may affect its usability for analysis and insight extraction. The better the quality of the dataset, the higher the utility to be derived for insight and robust decision making. For this purpose, one dataset was provided. This dataset with one table ‘marketing’ has 11 columns. A quality check validated all columns at 100%; zero errors and zero empty cells.
<img width="689" height="149" alt="image" src="https://github.com/user-attachments/assets/fb3d6353-cc19-4b93-a0e9-587b9f49ff70" />
<img width="810" height="259" alt="image" src="https://github.com/user-attachments/assets/c26d93ad-971a-484d-bb5f-fe93d348e543" />
The columns also bore the accurate datatype.

DATA INSIGHTS
This stage involves exploring, analysing and visualizing the data to understand patterns and trends which would further help in identify insights and potential variables for building a model. This stage is divided into two phases: Data Exploration & Modelling and Insights and Interpretation.
a) Data Exploration & Modelling: During data exploration, a date dimension table, dimDate, was created to enable detailed temporal analysis. The model is structured with dimensional tables and a fact table: dimDate includes Date, Year, Month, Quarter, Month Number, Day of the Week, and Week Number; dimProduct captures Product Name and Category; dimChannels records Marketing Channel; and the fact table fMarketing retains key metrics such as Ad Spend, Impressions, Clicks, Conversions, ROI, Revenue, Campaign Date, and CampaignID. This separation of descriptive attributes from quantitative metrics ensures efficient querying and a clear framework for analysis.
Certifying that the data is clean, and ready for interpretation, I established a connection between the four datasets using Power BI model feature to gain a deeper understanding of relationships and uncover insights.
<img width="1063" height="488" alt="image" src="https://github.com/user-attachments/assets/b49c5b3d-c0ee-4fb3-a061-60b6108cac83" />

a) Insights and Interpretation:
Insights drawn will be used to respond to the different preformulated requests below:
1. KPIs using Card Visuals:
   a. Total Ad Spend
<img width="585" height="216" alt="image" src="https://github.com/user-attachments/assets/98e78133-64f2-43c1-b76e-a232346749a4" />

A new measure was crafted (see attached above) to create the KPI card to total expenses on advertising. It amounted to 2.21 million (Indian Rupees)
<img width="164" height="96" alt="image" src="https://github.com/user-attachments/assets/8388e54d-dd48-41f8-81c3-e5908142c476" />
b. Impressions: This metric measures the reach of each campaign deployed.
<img width="166" height="104" alt="image" src="https://github.com/user-attachments/assets/8316bbdb-ef39-42c4-9601-d803aa0ac382" />

The figure for total impressions is at 221 million
c. Clicks: This metric represents the total number of times users interacted with a campaign, such as clicking on an ad or link. It reflects user engagement and helps measure the effectiveness of campaign reach in driving interest or traffic.
<img width="676" height="223" alt="image" src="https://github.com/user-attachments/assets/7910e1a9-b0d0-4da0-9e40-cf4f406fc0ea" />

CTR is gotten by dividing the total number of clicks by total number of impressions.
<img width="159" height="104" alt="image" src="https://github.com/user-attachments/assets/a3afd7dc-4628-4a9a-b3f2-b60b8a725476" />
A CTR of 5.13% means that out of all the times the campaign was shown (impressions), 5.13% of viewers clicked on it. In other words, for every 100 times the ad was displayed, about 5 people engaged by clicking, indicating the campaign’s effectiveness in attracting user attention.
d. Conversions: This metric measures the number of desired actions completed by users, such as purchases or sign-ups, indicating the effectiveness of a campaign in driving tangible results.
<img width="168" height="98" alt="image" src="https://github.com/user-attachments/assets/3ec6de23-39bb-4bde-b3cd-77774731d4c4" />

The conversion rate is 9.75%, calculated by dividing conversions by clicks. See the formula below:
<img width="667" height="230" alt="image" src="https://github.com/user-attachments/assets/a0c673cc-d9ed-41fe-9e3b-b351600531c6" />

e. Revenue: This metric represents the total monetary value generated from a campaign, reflecting the financial effectiveness and sales impact of marketing efforts.
<img width="155" height="94" alt="image" src="https://github.com/user-attachments/assets/a90137b2-cdca-4a38-8464-ffbd50a429ac" />

Total Revenue is 312 million Rupees (INR)
f. Overall ROI: This metric measures the efficiency or profitability of a campaign by comparing the revenue generated to the cost of running it. In plain terms, ROI is calculated as: ROI = (Revenue – Ad Spend) ÷ Ad Spend. It shows how much profit was made for each unit of money spent on advertising.
Attached are the formular and the KPI Card:
<img width="759" height="172" alt="image" src="https://github.com/user-attachments/assets/8d74666b-69d3-4c95-8eb3-b41dbe828b89" />

An ROI of 14,000% (or 14.0k%) means that for every 1 unit of currency spent on the campaign, 140 times that amount was earned in revenue. In other words, the campaign generated extremely high returns compared to its cost, indicating it was highly profitable.
<img width="181" height="115" alt="image" src="https://github.com/user-attachments/assets/03d6ad6a-2e79-413f-8532-def48f71700d" />

2.Visuals:
g. Ad Spend by Channel
<img width="436" height="293" alt="image" src="https://github.com/user-attachments/assets/287f4958-4649-4e53-b3de-faf367d26401" />

Key Findings: The marketing channel with the highest ad spend is Referral, closely followed by Google Ads, both around 0.48–0.49 million. Email Campaigns, Influencer Marketing, and Instagram Ads had slightly lower spends, ranging from 0.41 to 0.42 million. This distribution indicates that the business is investing heavily in referral programs and paid search, while social media and email campaigns receive comparatively moderate budgets. It suggests a strategic focus on channels that are likely driving the most measurable traffic or conversions, with room to assess the ROI of lower-spend channels for potential optimization.
h. Clicks vs Impressions
<img width="1364" height="362" alt="image" src="https://github.com/user-attachments/assets/ba748256-a39b-4e18-a906-7a9edceba7f7" />

Key Findings: The chart shows a consistent trend of impressions being significantly higher than clicks throughout the observed period (November 2024 to January 2025). This is a standard pattern, as impressions represent ad visibility while clicks represent user engagement.
i.
Conversion Rate by Category
Key Findings: The Conversion Rate by Category chart provides a breakdown of how well different product categories are converting. The data shows that the "Household" category has the highest conversion rate at 11.23%. This is a strong performance indicator, showing that a high percentage of visitors who interact with Household-related ads or content are completing a desired action, like a purchase. The strong conversion rate for the "Household" category also indicates a high potential for revenue.
j.
Revenue by Product
Key Findings: The top-performing products are "Cold Drink," "Dishwasher Liquid," and "Biscuits," each generating a substantial ₹18 million in revenue. These products are the primary revenue drivers for the business. Following closely, "Cooking Oil" and "Garbage Bags" contribute significantly with ₹17 million each. Products such as "Floor Cleaner," "Air Freshener," and "Eggs" also show consistent performance, each bringing in ₹16 million.
k.
ROI by Product/Category,
Key Findings: Air Freshener is the most profitable product with an exceptional return on investment of 24,933.7%. This indicates that for every unit of cost, this product generates a significantly higher profit than any other item. Eggs and Biscuits also perform remarkably well, with ROIs exceeding 19,000%, showcasing their strong profitability. While at the lower end of the listed products, Rice and Juice still demonstrate very healthy returns above 15,000%. The overall finding is that the entire product line presented in the chart is highly profitable, with Air Freshener being the clear standout in terms of efficiency and return on investment.
l.
Time-based trends for Spend, Conversions, ROI, and Clicks.
4.
Interactivity: Add slicers for Campaign Date, Product Name, Product Category, and Marketing Channel.
5.
DAX Measures: Create calculated fields for:
m.
CTR (Click through Rate)
n.
Conversion Rate
o.
ROI (double-check vs dataset ROI).
Interpretation: The table highlights a crucial difference between Overall ROI and Summed ROI in the dataset. Overall ROI, which is calculated as (Total Revenue – Total Spend) ÷ Total Spend, reflects the true profitability of each category because it accounts for the actual weight of spend and revenue in the calculation. For instance, if Beverages generated significant revenue compared to its spending, the Overall ROI correctly captures that efficiency.
In contrast, Summed ROI simply adds up ROI percentages from each row or transaction. Since ROI is a ratio rather than an absolute value, summing it across rows produces extreme and misleading results, often running into millions of percent. For example, Beverages shows a “Summed ROI” of over 5,000,000%, which dramatically overstates performance compared to the more realistic Overall ROI of about 13,000%.
