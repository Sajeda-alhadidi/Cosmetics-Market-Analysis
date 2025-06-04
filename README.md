HealthMax is a market leader in the shampoo industry, we have conducted an analysis
to come with actionable insights to grow the business.

data : 

<img width="530" alt="image" src="https://github.com/user-attachments/assets/c89c304b-ee52-47be-9200-855cd18743d7" />

this data contained the unit and value sales for a brand, sold in a specific region, during a specific month and year. Every brand belongs to only one subcategory and only one supplier.

First we conducted a Brands per Supplier analysis:

<img width="165" alt="image" src="https://github.com/user-attachments/assets/a2b2e766-4df1-403d-9a68-58941084dd80" />

here an overview of the different brands per supplier been created using PivotTable, as we can see healthmax has owned 2 brands in the market.

Year-over-year growth analysis :

<img width="228" alt="image" src="https://github.com/user-attachments/assets/c8b4ee8a-6e63-4c9b-ac88-b27c333805d8" />

Healthmax has evolved over the last couple of years, we created a PivotTable in a new worksheet, the value sales per brand for all years insighted the year 2020 had the strongest growth for both brands.

Year-to-Date :
we have created Year-To-Date (YTD) for all the dataset points as it shows below:

<img width="776" alt="image" src="https://github.com/user-attachments/assets/4a26ffc8-908f-4b96-996b-13ab59d3f76d" />


we have calculated the yearly total on the most granular level: unit sales by brand by region by year (Units YTD), using SUMIFS() function, as

Units YTD Formula =SUMIFS(H:H,D:D,[@Brand],E:E,[@Region],F:F,[@Year],G:G,"<="&[@Month])
Values YTD Formula =SUMIFS(I:I,D:D,[@Brand],E:E,[@Region],F:F,[@Year],G:G,"<="&[@Month])

This was purposed toward understanding how things are going throughout the year, then comparing values to previous months to track performance and make informed decisions.

Moving Annual Total :

<img width="778" alt="image" src="https://github.com/user-attachments/assets/93d0f242-ded1-4782-a3a5-16819c538ae8" />


we have calculated MAT which is the sum of the latest 12 months. where :

Units MAT Formula =[@[Units YTD]]+SUMIFS(H:H,D:D,[@Brand],E:E,[@Region],F:F,[@Year]-1,G:G,">"&[@Month])
Values MAT Formula =[@[Values YTD]]+SUMIFS(I:I,D:D,[@Brand],E:E,[@Region],F:F,[@Year]-1,G:G,">"&[@Month])


then the total turnover (revenue) of the total shampoo category been created using a PivotTable by employing the MAT values we calculated. 

<img width="187" alt="image" src="https://github.com/user-attachments/assets/e00105b2-de07-4c95-9724-6a3b0769990f" />

Market Share :
to identify the market share of the biggest players on the market. We have created a graph to see how our brands evolved over the years aand detect the regional differences.


<img width="670" alt="image" src="https://github.com/user-attachments/assets/ae967eb2-8732-411a-a658-6e94753598e8" 

  As HealthMax owns Starbust and Shinez. Starbust has 22% of market share in the South and is performing better in the South than in the rest of the country. For the Shinez, outperforms all competitors in the South and boasts the highest market share in 2023.

  Net Revenue Management :

  We have been asked to to make a list of product prioritizations in function of their net sales and their profitability, so we calculated the net sales for each product in 2022 where Total net sales for Healthmax product in 2022 was $20,480,715.

<img width="526" alt="image" src="https://github.com/user-attachments/assets/366bdd4a-d8d1-4037-ba19-7881e2e5a7fc" />


  Gross Margin :

  We  have created Gross Profit per unit to calculate HealtMax’ gross profit per unit for all products.

  <img width="886" alt="image" src="https://github.com/user-attachments/assets/2c6a442c-484c-429f-9a8c-63b39e6c5bc1" />

Heathmax’s portfolio has shown 68.49% of the average net selling price is gross profit.

Profitability Matrix :

To determine the percentage contribution of each product’s net sales to the total net sales for the year 2022, we have created a new column to your table called “Net Sales Contribution”, then the scatter plotting  it, so we can see that Starbust Ultra Soft 100ML is the most important product in the assortment with high contribution and high margin. In the same time, the Strong Hair range is situated at the bottom left corner of the scatter plot, meaning relatively low profitability and net sales.


<img width="440" alt="image" src="https://github.com/user-attachments/assets/2e87a06e-05ce-47d2-980f-990e114f251e" />

New Category Opportunity :
To identify the fastest growing category, we created a new pivot table to identify the subcategory that realized the biggest growth when comparing 2022 to 2018, This has indicated that  The biggest growth subcategory in 2022 is Organic shampoo.


<img width="309" alt="image" src="https://github.com/user-attachments/assets/21d73d02-fba0-4dac-9e12-4f57a7486db6" />

Our estimated values of organic shampoo sales in 2024 will be 1,020,899


<img width="274" alt="image" src="https://github.com/user-attachments/assets/5bddd55d-d3f6-4d9b-b90d-5bf970981203" />

New Product Launch :

as organic shampoo’s are blooming, HealthMax has two possible products that fit in this category and that can be launched in the beginning of 2024. to identify the best candidate by making an estimation of expected net sales, gross profit, and gross margin for both products.

<img width="289" alt="image" src="https://github.com/user-attachments/assets/eeae71f1-da1e-40ea-8c09-7e8dcca2ae47" />

Make an estimation of the Net Sales per product from Net Price :

<img width="712" alt="image" src="https://github.com/user-attachments/assets/48185b2e-150a-484e-bb0e-553d7fd21f85" />

insighted from above data, launching Herbashine will generate less net sales than HerbEssentials, but more gross profit.

Optimizing Net Revenue :
we have created the potential of a smaller shampoo bottle of 50ml, defining the retail price as 50% mark-up of the Price per ml of the 100ml pack. 
formula will look like this: =[@[Pack Size (ml)]]*E2*1.5
Defining the Net Price is $2.30 and the COGS amount to $0.70.

<img width="877" alt="image" src="https://github.com/user-attachments/assets/9fbb50a9-a627-40c7-bd7a-4f868cd6b1c0" />

Starbust Ultra Soft 50ml would generate $265,960 yearly.


Promotion Management :
HealthMax played three different promotions on the Shinez brand in 2022. To build the strategy for 2024, we calculated the ROI for the three different promotions.

<img width="173" alt="image" src="https://github.com/user-attachments/assets/d960d10b-5ac0-4677-95e7-44efaa304c92" />

The Promotion Graph comes with clear recommendations of which promotions are the most effective ones.

<img width="356" alt="image" src="https://github.com/user-attachments/assets/d58b7c98-1a50-402a-9db2-7891be0eaf6f" />

the #2 promotion is the most effective one as The ROI for this promotion is 12% and is higher than Promotion #3. The ROI of Promotion #1 is negative and should not be repeated.

<img width="595" alt="image" src="https://github.com/user-attachments/assets/68426d40-62aa-4176-8a50-628913cd73bd" />

Forecasting :
We will base ourselves on the market sales until 2022, extrapolate the current trend until 2024 and calculate what it represents in net sales. then the waterfall graph will present the numbers of forcastings.

Forecast table :
<img width="504" alt="image" src="https://github.com/user-attachments/assets/5de68899-7422-46af-aa20-ab40660a40e7" />


<img width="362" alt="image" src="https://github.com/user-attachments/assets/3190ad73-3c65-46c6-95c7-1c804b156904" />

with two Forecasted net sales for HealthMax in 2023, and 2024 estimated to be  $20,606,058 and $20,808,712 respectively.

As founded some great NRM opportunities to generate more net sales in follow our recommendations on “Mix Management” and “Promotion Management” , the waterfall chart indicated that NRM initiatives generate more net sales than the natural growth.



<img width="644" alt="image" src="https://github.com/user-attachments/assets/93bab0cb-8bb0-4f43-b295-9bec4eaae8f9" />







