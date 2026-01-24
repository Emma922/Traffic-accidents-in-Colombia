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
[R complete analysis](https://github.com/Emma922/Olist-Project/blob/302c4819153578439040c44af7a7dab13978ef14/Olist_EDA_cleaning.ipynb)



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


### Vehicle Type
-Motorcyclists account for over 70% of the 280 fatalities (232 cases), far exceeding cyclists (36) and automobile drivers (12).
- They show the highest risk across genders and are linked strongly to various accident types (chi-square p=2.652e-11 with victim characteristics).
- Cyclists mainly suffer collisions where not at fault (e.g., struck by vehicles).
​

## Insights Deep Dive

### Vehicle Type

- Motorcyclists account for over 70% of fatalities (232/280), far exceeding cyclists (36) and car drivers (12).
- Motorcyclists show the highest risk across genders and accident types (chi-square p=2.652e-11 with victim characteristics).
- Cyclists are primarily struck victims; rarely cause collisions themselves.
- Rollovers are more frequent among motorcycles on weekends.

### Age

- Fatalities concentrate among young adults; age distribution is positively skewed and non-normal (Shapiro-Wilk p=3.164e-11).
- The average age of motorcyclists involved in accidents is under 35 (t-test p=0.01322).
- Significant differences in average age exist between male and female victims (t-test p=0.0391).
- Young adults are disproportionately involved in high-risk accident types, especially motorcyclists and cyclists.

### Gender
- Men represent 88% of victims (247 vs. 33 women); fewer than 20% of victims are female (prop-test p=0.0003875).
- No significant associations were found between gender and accident type or between gender and victim characteristics (chi-square tests not rejected).
- Highlights higher male exposure and risk-taking behavior rather than structural factors.

### Accident Type & Class
- Types include collisions (fixed/moving objects, general) and rollovers, all fatal in the dataset.
- Strong association exists between accident type and victim characteristics (p=2.652e-11).
- Moving-object collisions peak on Saturdays (high traffic volume).
- Fixed-object collisions peak on Sundays (likely linked to impairment).
- Rollover incidents are most frequent on weekends.

### Victim Characteristics

- Dataset focuses on drivers; motorcyclists are the most vulnerable group.
- Cyclists are mostly struck victims rather than causing accidents.
- Victim type is independent of the day of the week (chi-square not rejected).
- No significant association between gender and victim type.
- Young males dominate the accident profile.

### Temporal Patterns 

- Significant variation in accident frequency by day of the week (chi-square p=2.167e-07).
- Saturdays show the highest number of moving-object collisions due to traffic density.
- Sundays show the highest number of fixed-object collisions, possibly related to alcohol or substance use.
- Rollovers increase significantly on weekends.
- Interventions should be tailored by day of the week to address peak-risk periods.

### Recommendations

- Target high-risk motorcyclists under 35: Helmets, training, and weekend awareness campaigns.
- Enhance weekend enforcement: Focus on Saturdays (traffic collisions), Sundays (impaired driving), and rollover monitoring.
- Protect cyclists: Infrastructure improvements, dedicated lanes, and driver awareness campaigns.
- Accident type-focused measures: Moving-object collisions (motorcyclists), fixed-object collisions (impaired drivers), rollovers (weekends).
- Age- and gender-specific interventions: Prioritize young males; adapt messaging where gender-neutral strategies apply.
- Temporal interventions: Adjust traffic control, checkpoints, and public campaigns based on day-specific risk patterns.
- Hotspot monitoring: Identify high-risk areas and use data-driven interventions to reduce accidents.
- Continuous evaluation: Regularly track accident patterns to refine interventions and identify emerging risk groups.
