# Cyclistic Bike-Share Analysis

## Project Overview
This project analyses Cyclistic bike-share usage from January to December 2025, comparing annual members and casual riders. Google BigQuery is used for data validation, cleaning and SQL analysis, while Tableau Public is used to visualise riding patterns and communicate business insights.

## Business Problem
Cyclistic wants to understand how annual members and casual riders use its bikes differently, so these patterns that can provide strategies to convert casual riders into annual members.

## Project Objectives
Compare monthly trip volume and average ride duration by rider type.
- Examine weekday and weekend riding behaviour.
- Compare demand and ride duration across seasons.
- Develop data-driven marketing recommendations.

## Tools and Technologies
- Google BigQuery 
- Tableau Public 
- Google Sheet and Google Connected sheets
  
Project Workflow

1. Validate the 12 monthly source datasets.
2. Clean records and calculate ride durations and calendar fields.
3. Analyse monthly trip volume and average ride duration.
4. Examine weekday and weekend behaviour.
5. Compare seasonal riding patterns.
6. Reconcile monthly, weekday and seasonal totals.
7. Build an interactive Tableau dashboard.
8. Document findings and business recommendations.

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

## Repository Structure
- `SQL/` — SQL scripts and technical documentation.
- `Visualisations/` — Tableau dashboard and chart screenshots.
- `Data/` — Dataset source and description.
- `Findings/` — Key findings and business recommendations.

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
