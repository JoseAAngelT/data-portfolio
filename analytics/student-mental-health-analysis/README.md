# Student Mental Health Analysis

## Overview

This project explores the relationship between length of stay in Japan and mental health indicators among international students.

Using descriptive analysis and data visualization, the study examines how depression, social connectedness, and acculturative stress vary across groups with different durations of residence.

## Objectives

* Analyze mental health indicators among international students.
* Compare average levels of depression, social connectedness, and acculturative stress by years of stay.
* Identify patterns associated with the adaptation process in a foreign environment.

## Dataset

Student Mental Health Dataset.

### Key Variables

| Variable | Description                        |
| -------- | ---------------------------------- |
| stay     | Length of stay in Japan (years)    |
| todep    | Depression score (PHQ-9)           |
| tosc     | Social connectedness score (SCS)   |
| toas     | Acculturative stress score (ASISS) |

## Tools

* Python
* Pandas
* DuckDB
* Matplotlib
* Seaborn
* Jupyter Notebook

## Methodology

* Filtered records to include only international students.
* Aggregated data by years of stay.
* Calculated descriptive statistics for mental health indicators.
* Visualized trends across residence-duration groups.
* Excluded groups with fewer than 10 observations from the main analysis to improve interpretability.

## Key Findings

* Most international students in the dataset had between one and four years of residence.
* Depression and social connectedness remained relatively stable across the analyzed groups.
* Acculturative stress showed a slight upward trend as years of stay increased.
* Groups with longer residence periods contained fewer observations, limiting the reliability of those estimates.

## Conclusion

The analysis suggests no substantial differences in depression or social connectedness across years of stay. However, acculturative stress appears to increase slightly over time within the observed population.

Given the descriptive nature of the analysis and the reduced sample size in some groups, the findings should be interpreted as exploratory rather than conclusive.