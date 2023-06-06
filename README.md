# EX-10-DataScience-Process-on-Complex-Dataset

# AIM:
To perform Data science process on a complex dataset and save the data to a file.

# ALGORITHM :

# STEP 1 :
Read the given Data 

# STEP 2 :
Clean the Data set using Data cleaning process 

# STEP 3:
Apply Feature Generation/Feautre Selection Techniques on the data set 

# STEP 4 :
Apply EDA/Data Visualization techniques to all the features of the data set

# PROGRAM :

DEVELOPED BY : THANIKA SREE B
REGISTER NUMBER : 212222100055
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt 
df = pd.read_csv('Air Quality.csv')
print(df.head())
print(df.describe())
print(df.isnull().sum())
df['Date'] = pd.to_datetime(df['Date']) 
plt.plot(df['Date']
         )
plt.title('Variation of air quality index over Time')
plt.xlabel('Date')
plt.show()
import pandas as pd
import matplotlib.pyplot as plt
plt.xlabel('Date')
plt.xticks(rotation=45)
plt.grid(True)
plt.show()
# a histogram of AQI values :
import seaborn as sns
plt.figure(figsize=(8, 6))
sns.histplot(data=df, bins=30, kde=True)
plt.ylabel('Frequency')
plt.show()
# a bar plot of AQI by location
plt.figure(figsize=(10, 6))
sns.barplot(data=df)
plt.xticks(rotation=45)
plt.show()
#  a line plot of AQI over time
df['Date'] = pd.to_datetime(df['Date'])
plt.figure(figsize=(10, 6))
sns.lineplot(data=df)
plt.xticks(rotation=45)
plt.show()
# a scatter plot of AQI by temperature
plt.figure(figsize=(8, 6))
sns.scatterplot(data=df)
plt.title(' Temperature')
plt.show()

# OUTPUT :

![ds 1](https://github.com/Thanikasreeb/EX-10-DataScience-Process-on-Complex-Dataset/assets/119557910/1d6b3100-fc5d-4a0e-967c-30eb81c41464)
![ds 2](https://github.com/Thanikasreeb/EX-10-DataScience-Process-on-Complex-Dataset/assets/119557910/450cc8d4-fd31-4201-897d-c401767e81c7)
![ds 3](https://github.com/Thanikasreeb/EX-10-DataScience-Process-on-Complex-Dataset/assets/119557910/aa09b30e-532b-47c9-9799-30713c88bee6)
![ds 4 1](https://github.com/Thanikasreeb/EX-10-DataScience-Process-on-Complex-Dataset/assets/119557910/c02c276f-cb77-4b72-8a8e-138ba830b83b)
![ds 5](https://github.com/Thanikasreeb/EX-10-DataScience-Process-on-Complex-Dataset/assets/119557910/4e8f9742-707c-4fcc-bd73-dfcbef4212ff)
![ds 6](https://github.com/Thanikasreeb/EX-10-DataScience-Process-on-Complex-Dataset/assets/119557910/d137575d-6bc6-48a0-abb0-835ac664dfb2)
![ds 7](https://github.com/Thanikasreeb/EX-10-DataScience-Process-on-Complex-Dataset/assets/119557910/0e0647d1-7a21-4054-8148-d277e6ba4a70)
![ds 8](https://github.com/Thanikasreeb/EX-10-DataScience-Process-on-Complex-Dataset/assets/119557910/26c9353f-9627-4706-9baf-b9b3457a53f2)
![ds 9](https://github.com/Thanikasreeb/EX-10-DataScience-Process-on-Complex-Dataset/assets/119557910/d75d387c-0291-406c-a2a5-8ee39e45bce8)

# RESULT :
 Thus , WE have read the given data and performed Data Science Process on complex dataset .









