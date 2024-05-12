## Electric Vehicle Charging Analysis

### Overview
This repository contains the code and analysis for the electric vehicle (EV) charging sessions dataset. The data includes information from 3,395 high-resolution charging sessions across 105 stations at 25 sites within a workplace charging program. The goal of this analysis is to gain insights into charging behavior and provide recommendations for optimizing workplace charging infrastructure.

## Dataset
**Data Format**: The dataset is available in CSV format

**Data Source**: [Electric Vehicle Charging Dataset on Kaggle](https://www.kaggle.com/datasets/michaelbryantds/electric-vehicle-charging-dataset/data)


**Variables**:
- **sessionId**: Unique identifier for each charging session.
- **kwhTotal**: Total kilowatt-hours (kWh) of electricity delivered during the session.
- **dollars**: Total cost of the charging session.
- **created**: Date and time when the session was initiated (likely in a format suitable for conversion to a datetime object in R).
- **ended**: Date and time when the session was terminated.
- **startTime**: Time of day the session began (might be separate from the created timestamp if the date information exists elsewhere).
- **endTime**: Time of day the session ended (might be separate from the ended timestamp if the date information exists elsewhere).
- **chargeTimeHrs**: Total duration of the charging session in hours.
- **weekday**: Day of the week (Monday, Tuesday, etc.) the session occurred.
- **platform**: Platform used to initiate or manage the charging session (e.g., mobile operating system, charging station interface).
- **managerVehicle**: Flag indicating whether the session involved a fleet vehicle managed by a company or organization.
- **facilityType**: Type of facility where the charging station is located (e.g., public parking garage, private residence).
- **Mon - Sun**: Binary flags indicating the day of the week (1 for that day, 0 otherwise). This might be redundant with the weekday variable.
- **reportedZip**: Zip code where the charging session was reported (might differ from the actual location if anonymized).


## Exploratory Data Analysis (EDA)
**1. Session Duration Distribution:**
  * Visualize the distribution of charging session durations.
  * Identify any outliers or patterns.

**2. Time of Day Analysis:**
  * Plot charging duration against time of day.
  * Look for peak charging hours.

**3. Insights**
  * Most charging sessions occur during typical work hours (9 AM to 5 PM).
  * Longer sessions are observed during lunchtime and at the end of the workday.
  * Some stations are consistently more popular than others.

