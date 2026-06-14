# NYC Public School SAT Performance Analysis

## Overview

This project analyzes SAT performance data from New York City public schools to identify high-performing schools in mathematics, determine the top schools based on combined SAT scores, and evaluate score variability across boroughs.

Using Python and Pandas for data analysis, the project explores academic performance patterns across NYC schools and boroughs through descriptive statistics and data visualization.

## Objectives

* Identify schools that achieved outstanding mathematics performance.
* Rank schools based on their combined SAT scores.
* Compare SAT score variability across NYC boroughs.
* Explore patterns in academic performance using descriptive statistics and visualizations.

## Dataset

NYC Public Schools SAT Performance Dataset.

### Data Dictionary

| Variable | Description |
|----------|-------------|
| school_name | Name of the public school. |
| borough | NYC borough where the school is located. |
| building_code | Unique school building identifier. |
| average_math | Average SAT Mathematics score. |
| average_reading | Average SAT Reading score. |
| average_writing | Average SAT Writing score. |
| percent_tested | Percentage of students who took the SAT. |

### Derived Variable

| Variable | Description |
|----------|-------------|
| total_SAT | Combined SAT score calculated as the sum of mathematics, reading, and writing scores. |

## Tools

* Python
* Pandas
* Matplotlib
* Seaborn
* Jupyter Notebook

## Methodology

* Loaded and inspected the dataset.
* Evaluated data quality and checked for missing values.
* Created a combined SAT score metric (`total_SAT`).
* Filtered schools that achieved at least 80% of the maximum SAT mathematics score.
* Ranked schools based on combined SAT performance.
* Calculated borough-level statistics, including average SAT scores and standard deviation.
* Visualized school rankings and SAT score distributions across boroughs.
* Interpreted findings to identify performance patterns.

## Key Findings

* Several NYC public schools exceeded the mathematics excellence benchmark of 640 points.
* Stuyvesant High School achieved the highest combined SAT score among all schools in the dataset.
* The top-performing schools recorded combined SAT scores above 2,000 points, reflecting consistently strong performance across all tested subjects.
* SAT score distributions varied across boroughs, with Queens and Manhattan showing greater score dispersion than other boroughs.
* High-performing outlier schools were present across multiple boroughs, indicating pockets of exceptional academic achievement throughout the city.

## Conclusion

This analysis identified schools with outstanding mathematics performance, ranked the highest-performing schools based on combined SAT scores, and examined score variability across NYC boroughs.

The findings highlight both exceptional academic achievement and differences in performance distributions across the city. While the analysis is descriptive in nature, it provides a concise overview of SAT performance patterns and can serve as a foundation for further investigation into factors associated with academic outcomes.