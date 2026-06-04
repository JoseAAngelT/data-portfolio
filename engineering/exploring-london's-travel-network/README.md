# Analyzing London Public Transport Usage with SQL

## Overview

This project analyzes passenger journey data from Transport for London (TfL) to explore usage patterns across different transport modes.

Using SQL queries executed with DuckDB, the analysis identifies the most popular transport services, examines peak demand periods for Emirates Airline, and investigates annual ridership trends within the London transport network.

## Objectives

- Identify the most popular transport modes based on total passenger journeys.
- Analyze peak ridership periods for Emirates Airline.
- Determine the years with the lowest demand for Underground & DLR services.
- Explore overall passenger demand trends across the TfL network.

## Dataset

Transport for London (TfL) Journeys Dataset.

### Key Variables

| Variable | Description |
|----------|-------------|
| MONTH | Month of the observation |
| YEAR | Year of the observation |
| DAYS | Number of days in the month |
| REPORT_DATE | Reporting date |
| JOURNEY_TYPE | Transport service category |
| JOURNEYS_MILLIONS | Passenger journeys (millions) |

## Tools

- Python
- Pandas
- DuckDB
- SQL
- Matplotlib
- Seaborn
- Jupyter Notebook

## Methodology

- Loaded and validated the dataset using Pandas.
- Queried the data using SQL through DuckDB.
- Aggregated passenger journeys by transport mode and year.
- Identified peak ridership periods for Emirates Airline.
- Analyzed annual demand patterns for Underground & DLR services.
- Visualized key results to support interpretation and communication of findings.

## Key Findings

- Bus was the most widely used transport mode, recording the highest cumulative passenger volume during the analyzed period.
- Underground & DLR accounted for the second-largest share of passenger journeys and showed notable variation in annual demand.
- Emirates Airline represented a relatively small proportion of total journeys, with peak ridership concentrated between 2012 and 2015.
- Annual passenger demand across the TfL network changed over time, revealing periods of decline and subsequent recovery.
- Passenger journeys were heavily concentrated in a small number of transport modes, particularly Bus and Underground & DLR.

## Conclusion

The analysis highlights the differences in passenger demand across London's transport network. Bus and Underground & DLR consistently carried the largest number of passengers, reinforcing their importance within the city's transportation system.

While Emirates Airline experienced isolated periods of higher demand, its overall contribution remained comparatively small. Additionally, annual ridership trends demonstrated that passenger volumes evolved over time rather than remaining constant.

Overall, the project demonstrates how SQL and DuckDB can be used to efficiently explore, aggregate, and analyze transportation data, transforming operational records into actionable insights.