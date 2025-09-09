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
## Main Goals
