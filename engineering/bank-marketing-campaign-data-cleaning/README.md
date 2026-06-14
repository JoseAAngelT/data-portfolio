# Bank Marketing ETL Pipeline

Cleaning, transforming, and restructuring marketing campaign data into relational tables using Python and Pandas.

## Overview

This project demonstrates a simple ETL workflow built with Python and Pandas.

A raw bank marketing dataset was cleaned, transformed, and separated into multiple logical tables to improve data organization and prepare the data for downstream storage and analysis.

The workflow includes data cleaning, type standardization, date engineering, validation checks, and CSV export.

## Dataset

The dataset contains information collected during a direct marketing campaign conducted by a banking institution.

Each record represents a client contacted during the campaign and includes:

* Demographic information
* Financial attributes
* Campaign interaction metrics
* Economic indicators

## Project Workflow

The following steps were performed:

1. Load the raw dataset.
2. Explore categorical variables and data types.
3. Clean and standardize categorical values.
4. Convert binary indicators to Boolean data types.
5. Create a standardized contact date field.
6. Separate the dataset into logical tables.
7. Validate output datasets.
8. Export transformed data to CSV files.

## Output Tables

### Client

Stores customer demographic and financial information.

| Field            | Data Type | Description                                               |
| ---------------- | --------- | --------------------------------------------------------- |
| `client_id`      | Integer   | Unique identifier assigned to each client.                |
| `age`            | Integer   | Client age in years.                                      |
| `job`            | String    | Type of occupation reported by the client.                |
| `marital`        | String    | Client marital status.                                    |
| `education`      | String    | Client education level.                                   |
| `credit_default` | Boolean   | Indicates whether the client has credit in default.       |
| `mortgage`       | Boolean   | Indicates whether the client has an active mortgage loan. |

### Campaign

Stores information related to marketing campaign interactions.

| Field                        | Data Type | Description                                                             |
| ---------------------------- | --------- | ----------------------------------------------------------------------- |
| `client_id`                  | Integer   | Unique identifier assigned to each client.                              |
| `number_contacts`            | Integer   | Number of contact attempts made during the current marketing campaign.  |
| `contact_duration`           | Integer   | Duration of the most recent contact, measured in seconds.               |
| `previous_campaign_contacts` | Integer   | Number of contact attempts made during the previous marketing campaign. |
| `previous_outcome`           | Boolean   | Indicates whether the previous marketing campaign was successful.       |
| `campaign_outcome`           | Boolean   | Indicates whether the current marketing campaign was successful.        |
| `last_contact_date`          | Date      | Date of the most recent client contact.                                 |

### Economics

Stores economic indicators associated with each client record.

| Field                  | Data Type | Description                                          |
| ---------------------- | --------- | ---------------------------------------------------- |
| `client_id`            | Integer   | Unique identifier assigned to each client.           |
| `cons_price_idx`       | Float     | Consumer Price Index (monthly economic indicator).   |
| `euribor_three_months` | Float     | Three-month Euribor rate (daily economic indicator). |

## Data Transformations

The following transformations were applied during the ETL process:

### Client Table

* Standardized categorical values using snake_case formatting.
* Replaced unknown education values with missing values (`NaN`).
* Converted `credit_default` and `mortgage` indicators to Boolean data types.

### Campaign Table

* Converted campaign outcome indicators to Boolean data types.
* Created a standardized contact date field using day, month, and year components.

### Economics Table

* Selected relevant economic indicators for export.

## Data Validation

Basic validation checks were performed before exporting the datasets:

* Dataset dimensions were verified.
* Client identifiers were checked for uniqueness.
* Data types were reviewed for consistency.
* Output tables were successfully generated.

## Technologies Used

* Python
* Pandas
* Jupyter Notebook

## Skills Demonstrated

* ETL Development
* Data Cleaning
* Data Transformation
* Data Validation
* Data Type Standardization
* Relational Data Preparation
* Data Export Automation

## Results

The original dataset was successfully transformed into three structured datasets:

* `client.csv`
* `campaign.csv`
* `economics.csv`

These outputs provide a cleaner and more organized structure for database storage and future analytical workflows.

## Conclusion

The original marketing dataset was successfully cleaned, transformed, and reorganized into separate client, campaign, and economics tables.

This project demonstrates fundamental data engineering practices, including data preparation, data type standardization, table restructuring, validation, and data export.
