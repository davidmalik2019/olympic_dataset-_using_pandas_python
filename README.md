# olympic_dataset-_using_pandas_python
Data cleaning and Visualization using pandas in python

The dataset contain some rows that were empty, so i had to       
(1) Cleaned the data by selecting the empty row and filling it with N/A and saved the new file as cleaned_row.csv in the data folder.

import pandas as pd
import matplotlib.pyplot as plt
import numpy as np
df = pd.read_csv('./data/cleaned_row.csv')
df.shape
new = df.dropna(how='all').fillna('N/A')
new.to_csv('latest_row.csv', index=False , na_rep='N/A')


(2) Sorted the cleaned data by selecting athlet that has height that is above 190 cm (height is advantage in some olympic games)

