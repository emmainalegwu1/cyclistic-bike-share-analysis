## SQL Documentation

## Overview

This folder contains the SQL scripts used to analyse the 2025 Cyclistic bike-share dataset. The analysis was conducted using Google BigQuery to examine differences in riding behaviour between annual members and casual riders.

The scripts are organised sequentially to demonstrate the data analysis process, from initial data validation and cleaning through to monthly, weekday and seasonal analysis.

## Dataset

- Project: my-project-52671-510211
- Dataset: Cyclistic_bikeshare
- Period: January – December 2025
- Source tables: 2025_01_divvy_tripdata to 2025_12_divvy_tripdata, https://divvy-tripdata.s3.amazonaws.com/index.html
- Licenece:  https://divvybikes.com/data-license-agreement

## SQL Scripts

## Script                     Description
01_data_validation.sql - Examines data completeness, row counts, distinct ride IDs, null values and invalid records.

02_data_cleaning.sql - Applies data-cleaning criteria, calculates ride durations and derives analytical fields.

03_monthly_analysis.sql - Compares monthly trip counts and average ride durations between members and casual riders.

04_weekday_analysis.sql - Examines trip volume and average ride duration across the seven days of the week.

05_seasonal_analysis.sql - Groups trips into four seasons and compares riding patterns by rider type.

06_final_validation.sql - Reconciles monthly, weekday and seasonal results to ensure consistency.

## Data Cleaning Criteria
The analysis applies the following criteria:

- Exclude records with missing ride IDs.
- Exclude records with missing rider classifications.
- Exclude records with missing start or end timestamps.
- Exclude rides lasting 30 seconds or less.
- Calculate ride duration using timestamp differences in seconds.
- Derive month and weekday classifications from the ride start timestamp.

The duration criterion is implemented using:

TIMESTAMP_DIFF(ended_at, started_at, SECOND) > 0

The same cleaning criteria should be applied consistently across monthly, weekday and seasonal analysis.

## Analytical Outputs

The SQL scripts generate the following analytical tables:

## Output table               Purpose

2025_month_trip_summary - Monthly trip counts and mean ride duration by rider type.

2025_weekday_trip_summary - Weekday trip counts and mean ride duration by rider type.

2025_seasonal_summary - Seasonal trip counts and mean ride duration by rider type.

## Execution Order

Run the scripts in the following order:

1. 01_data_validation.sql
2. 02_data_cleaning.sql
3. 03_monthly_analysis.sql
4. 04_weekday_analysis.sql
5. 05_seasonal_analysis.sql
6. 06_final_validation.sql

The output tables are subsequently used in Tableau Public to develop the project's visualisations and interactive dashboard.

## Validation

Final validation checks include:

- Comparing annual monthly trip counts against seasonal trip counts.
- Confirming that members and casual riders totals reconciles with month total.
- Comparing weekday trip counts against monthly totals.
- Investigating differences resulting from data cleaning or filtering.
- Ensuring that the mean ride durations are calculated from individual valid trips rather than by simply averaging monthly averages.

## Tools

- Google BigQuery
- Google Connected Sheets
- SQL (GoogleSQL)
- Tableau Public
