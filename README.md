# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 04/03/2025

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

```
import pandas as pd
import matplotlib.pyplot as plt

data=pd.read_csv("C:/Users/SEC/Downloads/kalimati_tarkari_dataset.csv/kalimati_tarkari_dataset.csv")

data['Date']=pd.to_datetime(data['Date'])
data.set_index('Date',inplace=True)

plt.figure(figsize=(10,6))
plt.plot(data.index,data['Average'],label='Average Price Today',color='brown')
plt.title('Average Price of vegetables')
plt.xlabel('Date')
plt.ylabel('Average Cost')
plt.grid(True)
plt.show()
```

# OUTPUT:

![image](https://github.com/user-attachments/assets/13d21456-d238-410e-bb03-1e7b15f1b14d)





# RESULT:
Thus we have created the python code for plotting the time series of given data.
