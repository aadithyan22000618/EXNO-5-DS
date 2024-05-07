# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

## Aim:
  To Perform Data Visualization using matplot python library for the given datas.

## EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

## Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

## Coding and Output:


> Developed By: AADITHYAN R

> REG NO: 212222230001
```py
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
```

### Line Plot:

```py
marks=[13,45,63,78]
student=['ABC','QOR','EFB','TOB']
plt.plot(marks,student)
plt.xlabel('Marks')
plt.ylabel('Student name')
plt.show()

student=['A','B','C','D']
attendence=[90,85,73,88]
plt.plot(attendence,student)
plt.xlabel('Attendence')
plt.ylabel('Student name')
plt.show()
```


![image](https://github.com/aadithyan22000618/EXNO-5-DS/assets/113586376/7e2fc93e-02c8-4b54-9296-cc0000a3fd44)
![image](https://github.com/aadithyan22000618/EXNO-5-DS/assets/113586376/c5753f1b-5339-48b0-8fc1-6729e764a9ac)



### Scatter Plot:

```py
x=[10,20,30,40,50]
y=[100,200,300,400,500]
plt.scatter(x,y,label='stars',color='green',marker='*',s=30)
plt.show()

x=np.arange(0,15)
y=np.arange(0,15)
x
y
plt.scatter(x,y,c='r')
plt.xlabel('X axis')
plt.ylabel('y axis')
plt.title('Scatter plot')
plt.show()
```
![image](https://github.com/aadithyan22000618/EXNO-5-DS/assets/113586376/8e8a63dc-82bf-4811-976d-4dc920d3bfa8)

![image](https://github.com/aadithyan22000618/EXNO-5-DS/assets/113586376/c22fcd03-df23-4d42-bf22-86d005cacc5c)





### Pie Chart:

```py
act=['eat','sleep','work','play']
slices=[3,7,8,6]
color=['r','y','g','b']
plt.pie(slices,labels=act,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()

feedback=['Good','excellent','Perfect','Ok']
slices=[4,10,3,8]
color=['y','r','b','g']
plt.pie(slices,labels=feedback,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
```

![image](https://github.com/aadithyan22000618/EXNO-5-DS/assets/113586376/9b35d237-8e88-4537-ba5c-2d1d86ff8724)

![image](https://github.com/aadithyan22000618/EXNO-5-DS/assets/113586376/32437b91-439e-4b96-84f9-60ecee41db91)



### Area Chart:

```py
x = [1, 2, 3, 4, 5]
y1 = [10, 12, 14, 16, 18]
y2 = [5, 7, 9, 11, 13]
y3 = [2, 4, 6, 8, 10]
plt.fill_between(x, y1, color='blue')
plt.fill_between(x, y2, color='green')
plt.plot(x, y1, color='red')
plt.plot(x, y2, color='black')
plt.legend(['y1','y2'])
plt.show()
```

![image](https://github.com/aadithyan22000618/EXNO-5-DS/assets/113586376/ae9398fc-f18a-4a53-b368-a0ff46e18cac)




### Bar Chart:

```py
height = [10, 24, 36, 40, 5]
names = ['one', 'two', 'three', 'four', 'five']
c1=['red', 'green'] 
c2=['b', 'g']
plt.bar (names, height, width=0.8, color=c1)
plt.xlabel('x - axis')
plt.ylabel('y - axis')
plt.title('My bar chart!')
plt.show()
```

![image](https://github.com/aadithyan22000618/EXNO-5-DS/assets/113586376/41e2742e-cac4-4073-b1bc-9766dca96158)



### Histogram:

```py
x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x, bins = 10, color='blue', alpha=0.5)
plt.show()
```

![image](https://github.com/aadithyan22000618/EXNO-5-DS/assets/113586376/9c41c00b-0855-4771-b93f-e32472038345)




### Box Plot:

```py
np.random.seed(0)
data=np.random.normal(loc=0, scale=1, size=100)
data
```

![image](https://github.com/aadithyan22000618/EXNO-5-DS/assets/113586376/112e0803-98f2-4e22-97b1-2e7385b7fbd0)



```py
fig, ax= plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```
![image](https://github.com/aadithyan22000618/EXNO-5-DS/assets/113586376/1465f775-d866-4ee7-9ac0-b62250e64a05)



## Result:

### Thus, all the data visualization techniques of matplotlib has been implemented.
