# Traffic accidents data Project

## Project Background

This academic project analyzes traffic accident data in Neiva Colombia between January 3, 2012, and January 31, 2022. The objective of the project is to identify key patterns and trends in the data that can provide actionable insights to support the development of effective traffic accident prevention campaigns.

## Dataset Overview

Data Source: [Traffic accidents dataset](https://www.datos.gov.co/dataset/MUERTES-ACCIDENTES-DE-TRANSITO-2012-2022-MARZO/wwir-6riq/data_preview)

Key Variables Analyzed:

Age of accident victims
Gender distribution
Type of vehicle involved
Day of the week
Type of accident/collision
Victim characteristics

**Insights and recommendations focus on the following key analytical areas:**

- **Category 1  Vehicle Type:**
Analysis of traffic accidents by vehicle type (e.g., motorcycle, automobile, truck, bicycle) to identify differences in accident frequency, accident type, and age, and to determine which vehicle categories are most strongly associated with high-risk outcomes.

- **Category 2 – Age:**
Examination of accident involvement by age group to identify demographic segments with higher accident frequency or severity, and to assess how age influences risk patterns across different types of traffic accidents and vehicle type.

- **Category 3 – Gender:**
Analysis of traffic accidents by gender to evaluate differences in accident rates, severity, and outcomes, with the aim of identifying behavioral or exposure-related patterns relevant to prevention strategies.

- **Category 4 – Accident Type & Accident Class:**
Assessment of accidents by type (e.g., collision, rollover, pedestrian involvement) and class (e.g., fatal, injury, property damage only) to identify the most common and most severe accident scenarios.

- **Category 5 – Victim Characteristics:**
Evaluation of victim-related factors such as role (driver, passenger, pedestrian), injury severity, and other available characteristics to understand vulnerability patterns and risk factors associated with traffic accidents.

- **Category 6 – Strategic Recommendations:**
Development of data-driven recommendations aimed at reducing traffic accidents and fatalities, supporting public safety policies, and guiding the design of targeted traffic accident prevention campaigns.


The R code to make the entire analysis and can be found here:  
[Python Cleaning and Exploration Code](https://github.com/Emma922/Olist-Project/blob/302c4819153578439040c44af7a7dab13978ef14/Olist_EDA_cleaning.ipynb)



## Executive Summary

### Overview of Findings

The analysis of traffic accident data in Colombia reveals clear patterns regarding accident frequency, victim characteristics, and risk factors. Motorcyclists and young adults emerge as the most vulnerable groups, while weekends—particularly Saturdays and Sundays—show significantly higher accident rates. The data also highlight strong relationships between certain accident types and victim characteristics, as well as differences in age distribution between genders.

Key insights include:

- Motorcycle drivers represent the highest risk group for traffic fatalities, accounting for more than 70% of all accidents.
- Women account for less than 20% of accident victims, confirming a significant gender disparity in traffic-related fatalities.
- The average age of motorcyclists involved in accidents is below 35 years, while the average age of accident victims differs significantly between men and women.
- Cyclists are primarily affected when they are struck by vehicles, rather than causing collisions themselves.
- Accident frequency varies significantly by day of the week, with Saturdays and Sundays showing the highest number of incidents. Collisions with moving objects peak on Saturdays, while collisions with fixed objects are more common on Sundays.
- Victim characteristics strongly correlate with accident type, but not with gender or the day of the week.
- There is no significant association between gender and accident type, nor between victim characteristics and gender.
- Rollover accidents are more frequent on weekends, suggesting a higher risk of loss of vehicle control during this period, likely influenced by alcohol or substance use.
- The chi-square analyses confirm several statistically significant relationships (e.g., accident type vs. victim characteristics, day vs. accident type), while other potential associations (gender vs. accident type, victim characteristics vs. day) were not significant.

### Recommendations Based on Findings

- Implement targeted road safety campaigns focusing on motorcyclists and young adult drivers, highlighting the heightened risk of weekend travel.

- Strengthen weekend traffic enforcement and monitoring, particularly on Saturdays and Sundays, to reduce collisions with moving and fixed objects.

- Promote cyclist safety programs, such as awareness campaigns and improved infrastructure, to protect vulnerable road users.

- Develop gender-informed road safety initiatives that consider differences in accident exposure and age-related risk patterns.

- Address rollover and high-risk accidents by implementing public campaigns against impaired driving and promoting safe driving behaviors on weekends.

- Use the findings to inform urban planning and traffic regulations, such as adjusting speed limits, traffic calming measures, and accident-prone zone interventions.

- Monitor accident trends over time to evaluate the impact of preventive measures and identify emerging risk patterns.
---

## Insights Deep Dive

### Historical Sales Performance

- All months show a consistent growth per year, indicating a general growth trend in sales per year.
This suggests that Olist has been strengthening its presence in the Brazilian market over time. 
  
- Based on the available data, we can infer that Olist may exhibit a seasonality pattern during the first 2 quarters of the year. However, due to the limited data across full yearly cycles, 
this conclusion cannot be confirmed with certainty. Since the dataset only extends to September 2018, we lack information on the final quarter of that year, preventing a complete comparison between first-quarter and last-quarter sales performance.

- The increase in sales observed during the first months of 2018 may be attributed to Olist�s overall growth rather than to a definitive seasonality pattern. 
With the current dataset, we cannot reliably distinguish between structural growth and seasonal effects.

![Customer Loyalty Snapshot](https://github.com/user-attachments/assets/a202a70e-f7f4-4bed-b4e2-0de7d446c750)



### Products and Category Performance

-  The data shows a strong **20–80 pattern**:
  - Only **7 out of 75** categories account for almost **50% of total sales**.
  - **21% of categories** represent **80% of total revenue**.
  - **17% of sellers** generate **80% of total sales**.
  - More than a half of sellers contribute **less than 5% of total revenue**.
  - **The top 10** sellers have different top 5 best-selling categories overall.
  - **The top 10** sellers generally rely heavily on one main category that generates the majority of their revenue


### Customer Behavior and Segmentation

- The "Best Customers" segment represents only 2% of the company's total revenue.
- "Potential Loyal Customers" contribute approximately one-fourth of total revenue, highlighting the importance of implementing loyalty-building initiatives.
- The "At Risk" segment accounts for nearly one-third of all customers, indicating that many previously frequent buyers are no longer generating sales.
- These findings underscore the importance of maintaining customer relationships over time to secure consistent and recurring revenue.
- Based on the RFM analysis, customers who contribute most  to the sales did not make additional purchases

Nr. Orders per Customer Viz
- This chart shows the dominance of single-purchase customers, which suggests low repeat purchase rates


![Nr. Orders per Customer](https://github.com/user-attachments/assets/8a2627b8-65f8-49cd-aa54-08d71a6871b2)

### Geographic Sales Distribution

- Beleza_saude appears in the top 5 categories in every state, indicating consistently strong performance
  and broad customer demand across the country.
- Cama_mesa_banho appears in the top 5 in only 8 out of 27 states, which suggests a more region-specific demand.
Addtionally, it is purchased mainly in the highest-revenue states, showing stronger demand in larger and more developed markets.
- Sao Paulo (SP) is the state with the highest overall revenue. It also shows high category diversification,
meaning its sales are distributed across many different product categories rather than concentrated in a few.
- Consumer preferences are relatively consistent across states, but purchasing power and market size vary significantly.
- States with the highest revenue also tend to have the largest number of sellers. In contrast, low-revenue states usually have very few sellers or in some cases, none, indicating that seller scarcity directly limits sales potential.

Sales Performance by State (to consult state details and accurate specific information please enter into the dashboard)


![State Performance](https://github.com/user-attachments/assets/fcf24d00-c86a-41f8-8dd3-95a2bdaf5edc)

### Review score and Service Quality

- Several sellers show low average ratings (<3.0), suggesting operational deficiencies such as late shipments, poor handling, or inconsistent service. 
These sellers should be monitored closely and may require training or performance improvement plans.

- Delivery delays significantly reduce customer satisfaction, as evidenced by the lower average review scores for delayed orders.
This reinforces the importance of logistics efficiency and accurate delivery-time estimates.

- Categories with both high sales volume and high review scores represent strong performance areas. 
In contrast, categories with low review scores signal opportunities for targeted service or product improvements.

- Moveis_escritorio is a high-priority category for intervention because it combines low review scores with high order volume, 
meaning a large number of customers are being negatively affected.

- Cama_mesa_banho is another key category: despite being among the highest in revenue and total orders, it also shows one of the lowest average review scores. 
This mismatch indicates a risk of long-term customer dissatisfaction in a high-impact category.

- Seller 7c67e1448b00f6e969d365cea6b010ab stands out as a critical case: despite selling over 1,300 products, 
the seller maintains the lowest average review scores, suggesting severe operational or quality-related issues.

- Improving logistics reliability and monitoring low-performing sellers could significantly raise customer satisfaction across the platform.

### Order payments type

- High-installment sellers vary significantly across product categories. 

- Categories like 'eletrodomesticos_2', 'moveis_decoracao', and 'automotivo' have the highest average installments, suggesting reliance on financing for higher-priced or durable goods.

- Customer financing preferences align with product type, particularly for expensive or long-term purchase items. 


## Recommendations

Based on the analysis, the following actions are recommended to the stakeholder team:

- **Expand market reach:** Leverage Olist’s steady growth with nationwide marketing campaigns to sustain momentum and attract new customers.
- **Activate inactive sellers:** Launch seller‑focused initiatives (training, incentives, promotional tools) to increase participation and revenue contribution.
- **Prioritize high‑performing categories:** Invest in marketing and inventory for top categories and products that consistently drive sales.
- **Optimize freight policies:** Balance shipping costs across states to reduce barriers in underperforming regions and boost demand.
- **Strengthen logistics and quality control:** Improve delivery reliability, monitor low‑rated sellers, and address product/service complaints to enhance customer satisfaction.
- **Leverage financing preferences:** Tailor marketing and payment options to categories where installment plans are most common, supporting higher‑value purchases.
- **Build customer loyalty programs:** Implement engagement strategies to encourage repeat purchases and reduce reliance on one‑time buyers.
