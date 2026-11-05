# Cyclistic Bike-Share Analysis

## Project Overview
This project analyses Cyclistic bike-share data to understand how annual members and casual riders use the company's bike-sharing services differently.

The analysis explores usage patterns over a 12-month period in 2025, with the aim of identifying insights that can help Cyclistic improve customer engagement and convert casual riders into annual members.

## Business Problem
Cyclistic wants to understand the differences between annual members and casual riders to develop more effective marketing strategies and increase annual membership.

## Project Objectives
- Analyse monthly trip patterns.
- Compare total trips by rider type.
- Compare mean ride durations.
- Identify differences in weekday usage.
- Examine seasonal riding patterns.
- Develop data-driven marketing recommendations.

## Tools and Technologies
- Google BigQuery – SQL data cleaning and analysis.
- Tableau Public – Data visualisation and dashboard development.
- Google Sheet and Google Connected sheets – Data preparation and supporting analysis.

## Data Preparation
The analysis uses 12 months of Cyclistic bike-share trip data.

Data preparation activities include:
- Accessing data from Amazon AWS cloud storage https://divvy-tripdata.s3.amazonaws.com/index.html
- Data licensing was through Motivate International inc., under the license https://divvybikes.com/data-license-agreement.
- Combining monthly datasets.
- Identifying and removing invalid ride records.
- Calculating ride durations.
- Categorising riders into members and casual users.
- Extracting weekdays, months and seasons for trend analysis.
  
## Data Processing
Data processing activities include:
- Identifying distinct values and removing errors.
- Cleaning and transforming the data to remove invalid ride data.
- Calculating ride durations in minute in Float 64 format.
- Categorising riders into members and casual users.
- Extracting weekdays, months and seasons for trend analysis.

## Analysis
The project examines:
1. Annual trip count
2. Annual trip count by user type.
3. Monthly riding behaviour.
4. Mean ride length.
5. Weekday riding patterns.
6. Seasonal riding behaviour.
7. Combining monthly datasets.

## Dashboard
(https://public.tableau.com/views/CyclisticBikeshareCasestudyViz/Dashboard1?:language=en-GB&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

## Key Findings
1. The analysis of the data shows that the difference in the usage of Cyclistics Bikes is that, annual members take more trips than casual riders because of the flexibility and freedom the membership offers them.
2. Casual riders on the other hand tend to have longer rides durations than annual members, so they can make the most of their single ride or full day pass payment.
3. From the analysis, the trend shows that members rode at any day of the week while casual riders rode most during the weekends, specifically, Saturday and Sunday.
4. Both Casual riders and annual members prefer riding season is summer. Which in Chicago are June, July and August.

## Business Recommendations
1. The marketing team is to make a campaign on the flexibility and freedom of using Cyclistic Bikes at their convenience by becoming annual members.
2. The membership subscription fee should be discounted for a limited time period for existing casual riders to enable easy membership type switching.

## Conclusion
This project demonstrates the application of SQL and data visualisation techniques to analyse customer behaviour and generate insights that can support business decision-making.
