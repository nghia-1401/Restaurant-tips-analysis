# Restaurant-tips-analysis
<img width="1000" height="563" alt="image" src="https://github.com/user-attachments/assets/10c428f1-dd4f-4e1d-8a7b-73d7b8d76c4d" />

This project aims to use the restaurant tips dataset to practice creating composition plots and visualizations. We will examine the relationship between different variables and the tips given.

## Data
### Data Source
The dataset comes from the Tips Dataset, originally introduced in Modern Applied Statistics with S (Venables & Ripley, 2002) and now available through the Seaborn library. It contains 244 observations and 7 variables related to restaurant bills and tips.
### Data Description
Number of observations: 244 obs
Number of variables: 7.
As you can see each observation represents a customer who left a tip at a restaurant.  

    total_bill: the total bill
    tip: số tiền tip (USD).
    sex: the sex of the person
    smoker: if they were a smoker or not
    day: the day it occurred
    time: if it was at lunch or dinner
    size: the size of the party
### Data Access
First, let's import the needed libraries: Pandas & Matplotlib.
```
import pandas as pd
import matplotlib.pyplot as plt
```
Then load data from the following link: https://raw.githubusercontent.com/RusAbk/sca_datasets/main/tips.csv
```
df=pd.read_csv('https://raw.githubusercontent.com/RusAbk/sca_datasets/main/tips.csv')
```
### Data exploration
#### Data Sample
```
df.head()
```
|index|id|total\_bill|tip|sex|smoker|day|time|size|
|---|---|---|---|---|---|---|---|---|
|0|0|16\.99|1\.01|Female|No|Sun|Dinner|2|
|1|1|10\.34|1\.66|Male|No|Sun|Dinner|3|
|2|2|21\.01|3\.5|Male|No|Sun|Dinner|3|
|3|3|23\.68|3\.31|Male|No|Sun|Dinner|2|
|4|4|24\.59|3\.61|Female|No|Sun|Dinner|4|
## Main Goals
The main objective of this project is to examine the factors influencing tipping behavior in restaurants. Specifically, the analysis tests for differences in tip amounts across:
    
    Smokers vs. Non-smokers
    Males vs. Females
    Weekends vs. Weekdays
    Dinner vs. Lunch
## Results
### Do people who smoke give more tips?
<img width="1789" height="490" alt="image" src="https://github.com/user-attachments/assets/5e268783-ef0c-4881-93b7-72278eb576b4" />

    1. Insight 1: Most customers give small tips (2–4 USD), and very few give large tips (>6 USD).
    2. Insight 2: The tip distribution of non-smokers is more even compared to smokers.
    3. Insight 3: Smokers tend to give lower and less diverse tips.

    Conclusion: Non-smokers generally give higher and more varied tips, while smokers tend to give smaller and less diverse tips. Overall, most customers tip in the range of 2–4 USD, with large tips above 6 USD being rare.
###  Do males give more tips?
<img width="1189" height="490" alt="image" src="https://github.com/user-attachments/assets/ee711482-4cbf-449a-bcbb-7fec18294650" />  

    Conclusion: Males tend to tip more and with greater variation, including some very high tips.
                Both males and females tip around 2 USD
