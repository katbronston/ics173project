# -*- coding: utf-8 -*-
"""
Created on Thu Dec 17 18:01:55 2020

@author: katbr

Created by Katherine Bronston
For ICS 173
Code written on 12/17/2020 and 12/18/2020
"""

# Import Libraries
import matplotlib.pyplot as plt
import pandas as pd

# Declare lists
date=[]
death=[]

# Declare the file path - r is needed to let address be a string. 
#Replace inside the '' marks as needed to change file path
covid_filepath = r'C:\Users\katbr\Documents\Python\hawaii-history.csv'

# Reads thedata from the csv file
covid_data = pd.read_csv(covid_filepath)

# Saves data from specific columns to lists
date = pd.to_datetime(pd.Series(covid_data['date']))
death = covid_data['death']  
 
# Plots dates on x axis, cumulative death total on y axis     
plt.plot(date,death, label='Statewide Deaths', linestyle='solid')

# Axis Labels
plt.xlabel('Month')
plt.ylabel('Cumulative Deaths')

# Plots months vertically so that axis tick marks are legible
plt.xticks(rotation='vertical')

# Plot title & legend
plt.title('Cumulative COVID-19 Deaths - Hawaii')
plt.legend()

# Actually graphs the data
plt.show()
