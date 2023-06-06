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
```
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
#a histogram of AQI values :
import seaborn as sns
plt.figure(figsize=(8, 6))
sns.histplot(data=df, bins=30, kde=True)
plt.ylabel('Frequency')
plt.show()
#bar plot of AQI by location
plt.figure(figsize=(10, 6))
sns.barplot(data=df)
plt.xticks(rotation=45)
plt.show()
#a line plot of AQI over time
df['Date'] = pd.to_datetime(df['Date'])
plt.figure(figsize=(10, 6))
sns.lineplot(data=df)
plt.xticks(rotation=45)
plt.show()
#a scatter plot of AQI by temperature
plt.figure(figsize=(8, 6))
sns.scatterplot(data=df)
title(' Temperature')
plt.show()
```
# OUTPUT :

![ds 1](https://github.com/Thanikasreeb/EX-10-DataScience-Process-on-Complex-Dataset/assets/119557910/d4285879-f201-42f6-8245-37d1df128876)
![ds 2](https://github.com/Thanikasreeb/EX-10-DataScience-Process-on-Complex-Dataset/assets/119557910/f16e4e9c-ad29-4d32-8bd5-10c5bbb6785f)
![ds 3](https://github.com/Thanikasreeb/EX-10-DataScience-Process-on-Complex-Dataset/assets/119557910/a8338e4c-3cec-4ede-ac77-7d87b787018d)
![ds 4](https://github.com/Thanikasreeb/EX-10-DataScience-Process-on-Complex-Dataset/assets/119557910/b100013b-e858-47fc-b2f0-33be37ea14bb)
![ds 5](https://github.com/Thanikasreeb/EX-10-DataScience-Process-on-Complex-Dataset/assets/119557910/2c26fc0d-6009-4cfe-bd1f-6546f1de84b8)
![ds 6](https://github.com/Thanikasreeb/EX-10-DataScience-Process-on-Complex-Dataset/assets/119557910/eea0fd8f-d4be-457a-8b00-49508e282a36)
![ds 7](https://github.com/Thanikasreeb/EX-10-DataScience-Process-on-Complex-Dataset/assets/119557910/5621613a-d2a8-4f56-9075-55b66f4b14a0)
![ds 8](https://github.com/Thanikasreeb/EX-10-DataScience-Process-on-Complex-Dataset/assets/119557910/ea1dd07c-e54e-439b-bf0a-d66f78bef4a5)
![ds 9](https://github.com/Thanikasreeb/EX-10-DataScience-Process-on-Complex-Dataset/assets/119557910/24cd10f3-f949-4b27-a5a8-76266f904e2e)

# RESULT :
 Thus , We have read the given data and performed Data Science Process on complex dataset .









