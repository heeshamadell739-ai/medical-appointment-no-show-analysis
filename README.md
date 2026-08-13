# Medical Appointment No-Show Analysis

## Project Overview

This project analyzes medical appointment data to understand the factors associated with patients missing their scheduled appointments.

The analysis focuses on appointment waiting time, SMS reminders, age, appointment weekday, medical conditions, and neighbourhood.

## Objectives

The main objectives of this project are to:

- Analyze the relationship between waiting time and no-show rates.
- Investigate the association between SMS reminders and appointment attendance.
- Examine whether age affects no-show behavior.
- Analyze no-show rates across appointment weekdays.
- Investigate the relationship between the number of medical conditions and no-shows.
- Identify neighbourhoods with relatively high and low no-show rates.
- Provide data-driven recommendations based on the findings.

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Data Preparation

The dataset was cleaned and prepared before analysis.

The main preprocessing steps included:

- Removing an invalid age value.
- Checking for missing values and duplicate records.
- Correcting data types.
- Converting date columns to datetime format.
- Checking categorical and binary variables.
- Removing records with negative waiting times.

## Feature Engineering

Several new features were created to support the analysis:

- `WaitingDays` — number of days between scheduling and the appointment.
- `WaitingCategory` — grouped waiting time into categories.
- `AppointmentWeekday` — day of the week of the appointment.
- `MedicalConditionCount` — number of recorded medical conditions.
- `IsNoShow` — numerical representation of the no-show outcome.
- `Age_Group` — grouped patients into age categories.

## Key Findings

The analysis found that:

- Longer waiting periods are generally associated with higher no-show rates.
- SMS recipients had a higher overall no-show rate, but the relationship changes when waiting time is considered.
- Younger age groups, particularly ages 10–29, showed relatively higher no-show rates.
- Appointment weekday showed relatively small differences in no-show rates.
- Patients with fewer recorded medical conditions showed higher no-show rates in this dataset.
- Neighbourhood showed noticeable variation in no-show rates.

The overall no-show rate in the analyzed data was approximately **22.08%**.

## Recommendations

Based on the analysis:

1. Prioritize patients with longer waiting periods for additional reminders.
2. Use SMS reminders strategically, particularly for appointments with longer waiting periods.
3. Investigate neighbourhoods with unusually high no-show rates.
4. Consider additional engagement strategies for younger patient groups.
5. Avoid making decisions based on groups with very small sample sizes.
6. Monitor both no-show rate and the total number of no-shows.

## Project Structure

```text
medical-appointment-no-show-analysis/
│
├── README.md
├── Week4_Assessment.ipynb
└──  Medical Appointment No-Show Analysis.ipynb
    └── KaggleV2-May-2016.csv
```

## Disclaimer

This project is an exploratory data analysis exercise. The observed relationships do not necessarily imply causation.
