# EXNO-6-DS-DATA VISUALIZATION USING SEABORN LIBRARY
## Name : SAJITH AHAMED F
## Reg No : 212223240144
# Aim:
  To Perform Data Visualization using seaborn python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:

```
import seaborn as sns
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=[1,2,3,4,5]
y=[3,6,2,7,1]
sns.lineplot(x=x,y=y,linestyle='dashed',color='blue')
plt.title("Line-chart")
plt.xlabel("x-axis")
plt.ylabel("y-axis")
plt.show()
```
![image](https://github.com/user-attachments/assets/dca4de51-5444-4ad7-a837-be3bf39bf248)
```
X = [1, 2, 3, 4, 5]
y1 = [2, 6, 4, 8, 9]
y2 = [4, 3, 5, 7, 1]
y3 = [6, 4, 3, 7, 9]
sns.lineplot(x=x,y=y1, color='red', linestyle='solid', linewidth=2)
sns.lineplot(x=x,y=y2,color='green', linestyle='dashed',linewidth=2)
sns.lineplot(x=x, y=y3, color='blue', linestyle='dotted', linewidth=2)
plt.title("Multi-Line chart")
plt.xlabel("x-axis")
plt.ylabel("y-axis")
plt.show()
```
![image](https://github.com/user-attachments/assets/9a5fd6d4-db56-4708-bb43-ff3ed6cc9d14)
```
df=sns.load_dataset('tips')
sns.barplot(x='day', y= 'total_bill',hue='sex', data=df,palette='Set1')
plt.title("Total bill by day and Gender")
plt.xlabel("Days of the week")
plt.ylabel("total bill")
```
![image](https://github.com/user-attachments/assets/bfa4ae2c-4e90-4c73-9ac4-dfb06527b921)
```
df=sns.load_dataset('tips')
df
```
![image](https://github.com/user-attachments/assets/518be219-62b0-4dd0-bc72-34a87227ea18)
```
sns.scatterplot(x='total_bill', y='tip', hue='sex',data=df)
plt.xlabel('total bill')
plt.ylabel('tip amount')
plt.title("Scatter plot of total bill vs tip Amount")
```
![image](https://github.com/user-attachments/assets/b824a4f3-1087-4256-b656-842be3057416)
```
sns.histplot(x='total_bill', hue='sex',data=df,kde=True)
plt.title("Histogram of Total Bill by Gender")
plt.xlabel("Total Bill")
plt.show()
```
![image](https://github.com/user-attachments/assets/6a67d92e-aea4-46c6-9c42-e553ba77f59d)
```
sns.kdeplot(x='total_bill', data=df,hue='sex',multiple='stack')
plt.title("Stacked KDE Plot of Total Bill")
plt.xlabel("Total Bill")
plt.show()
```
![image](https://github.com/user-attachments/assets/6cb3d10b-0c37-4a4b-919b-6f643e59f674)
```
sns.boxplot(x='day',y='total_bill',hue='smoker',linewidth=2,width=0.6,data=df)
boxprops={'facecolor': 'lightblue', 'linestyle': '-', 'linewidth':1.5},
whiskerprops={'color': 'black', 'linestyle': '--', 'linewidth':1.5},
capprops={'color': 'black', 'linestyle':'--', 'linewidth':2}
```
![image](https://github.com/user-attachments/assets/13115208-24ea-4d4f-a7f3-0d2d0f0f8684)
```
sns.violinplot(x='day',y='total_bill',hue='smoker', data=df, linewidth=2,width=0.6)
plt.title("Violin plot")
plt.xlabel("Days of the week")
plt.ylabel("total Bill")
```
![image](https://github.com/user-attachments/assets/474f838a-f7fc-4c93-8b18-858de42734e7)
```
corr = df.corr(numeric_only=True)
sns.heatmap(corr, annot=True, cmap="coolwarm", linewidths=0.5)
plt.title("Correlation Heatmap")
plt.show()
```
![image](https://github.com/user-attachments/assets/92038c43-2eca-44b4-b04f-1536169e1e46)
```
sns.pairplot(df, hue='sex', palette='husl')
plt.suptitle("Pairplot of Tip Dataset", y=1.02) 
plt.show()
```
![image](https://github.com/user-attachments/assets/4aeefbc8-21a5-4181-a2e4-c5581ddb8b2d)


# Result:
Data Visualization using seaborn python library is successfully completed.
