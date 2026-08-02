

# Telcommunication Customer's Predictions

Automates the cleaning and preprocessing of raw telecommunication customer data. It removes unnecessary demographic and feature columns, drops duplicate rows, handles missing values, and saves as a clean dataset for analytical or modeling use.


## KeyPoints

1. Tenure:  Number of months a customer has stayed with the company. With a very high concentration of brand-new customers (0–10 months) and long-term customers (over 65 months).
   
3. MonthlyCharges: Amount billed to the customer each month, showcasing a massive cluster of customers paying the bare minimum rate (around $20–$25 per month).
   
4. TotalCharges: Total revenue collected from each customer (tenure multiplied by MonthlyCharges).


- Drops 15 operational and demographic columns to isolate core customer metrics
- Identifies and eliminates identical data entries
- Filters out incomplete rows to ensure data integrity


#### Prerequisites

`Python3`

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
  
5. Filters out rows containing missing values (`NaN`)
   
6. Overwrites `telco-customer-churn.csv` as final, optimized dataset



## Visualization





##### Note

> Installed Anaconda
> Jupyter Notebook
