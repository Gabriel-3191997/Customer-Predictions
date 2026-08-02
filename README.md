

# Telcommunication Customer's Predictions

Automates the cleaning and preprocessing of raw telecommunication customer data. It removes unnecessary demographic and feature columns, drops duplicate rows, handles missing values, and saves as a clean dataset for analytical or modeling use.

## Features

- Drops 15 operational and demographic columns to isolate core customer metrics
- Identifies and eliminates identical data entries
- Filters out incomplete rows to ensure data integrity

## Prerequisites

`pandas` 
`matplotlib`


```bash
pip install pandas
```

```bash
pip install matplotlib
```


## Dataset

 `telco-customer-churn.csv`

[Reference]: (https://www.kaggle.com/datasets/yeanzc/telco-customer-churn-ibm-dataset)
 
## Workflow

1. Loads the raw CSV file into a pandas DataFrame
   
3. Eliminates the following categorical columns:
   - `SeniorCitizen`, `Partner`, `Dependents`
   - `PhoneService`,
   - `InternetService`,
   - `MultipleLines`,
   - `OnlineSecurity`,
   - `OnlineBackup`,
   - `DeviceProtection`,
   -  `TechSupport`,
   -  `StreamingTV`,
   -   `StreamingMovies`
   - `PaperlessBilling`,
   - `PaymentMethod`,
   - `Churn`
     
4. Drops duplicate records
5. Filters out rows containing missing values (`NaN`).
6. Overwrites `telco-customer-churn.csv` with the final, optimized dataset.

## Usage

Run the script from your terminal or IDE:

```bash
python clean_churn_data.py
```

##### Note

> Installed Anaconda
> Jupyter Notebook
