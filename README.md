# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 

# AIM:
To Develop a python program to Plot a time series data (population/ market price of a commodity
/temperature.
# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Calculate the mean for the respective column.
4. Plot the data according to need and can be altered monthly, or yearly.
5. Display the graph.
# PROGRAM:
###
```
import pandas as pd
import matplotlib.pyplot as plt

# Sample time series data
data = {
    'Date': ['2026-01-01', '2026-02-01', '2026-03-01',
             '2026-04-01', '2026-05-01', '2026-06-01'],
    'Sales': [100, 120, 150, 130, 180, 200]
}

# Create a DataFrame
df = pd.DataFrame(data)

# Convert Date column into datetime format
df['Date'] = pd.to_datetime(df['Date'])

# Plot the time series
plt.figure(figsize=(10, 5))
plt.plot(df['Date'], df['Sales'], marker='o')

# Add title and labels
plt.title('Time Series Plot of Sales')
plt.xlabel('Date')
plt.ylabel('Sales')

# Display grid
plt.grid(True)

# Show the plot
plt.show()

```
###
# OUTPUT:
<img width="1087" height="552" alt="image" src="https://github.com/user-attachments/assets/8a328948-47ad-40fb-8546-525b11649241" />






# RESULT:
Thus we have created the python code for plotting the time series of given data.
