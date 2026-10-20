I built this project to practice doing a full analysis inside Power BI, from importing the raw files to making the final dashboard. I used the Olist Brazilian e-commerce dataset from Kaggle, which has around 100k orders from 2016 to 2018 spread across 9 tables.

**Dataset: https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce**

**What I wanted to find out**
How does revenue change month to month?
How do customers pay, and which payment type brings in the most revenue?
Which states generate the most revenue?
How happy are customers, and how much does an average order cost?
**What I did**
1.)Cleaned the data in Power Query (data types, blanks, duplicate columns)
2.)Connected the 9 tables into a data model with the orders table in the middle
3.)Made a Calendar table for the time analysis
4.)Wrote DAX measures for gross revenue, net revenue, average order value and average review score
4.)Designed the dashboard with a custom dark theme, KPI cards and Year and Quarter slicers
**A few things I noticed**
1.)Revenue grew a lot through 2017 and peaked in November 2017, probably because of Black Friday.
2.)From early 2018 it stayed flat at around R$1.0 to 1.2M a month.
3.)The data is very thin before 2017 and after August 2018, so I only looked at Jan 2017 to Aug 2018. Otherwise the trend line drops to zero at the end, which isn't a real drop.
4.)At first my chart used month names on the axis and showed a fake drop, because Jan to Aug had two years of data added together and the other months only had one. Using Year-Month fixed it.

All revenue numbers are in Brazilian reais and include freight. They show what customers paid, not Olist's own income.

**Tools:**
Power BI, Power Query, DAX
