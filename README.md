# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

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
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
```
Line Plot:
```
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

<img width="1008" height="728" alt="image" src="https://github.com/user-attachments/assets/4c008fcf-c23a-4b2d-a857-a0fe823b1efe" />
<img width="956" height="739" alt="image" src="https://github.com/user-attachments/assets/4a6d16a8-06b4-4427-a4a1-11e10f8d8685" />

Scatter Plot:
```
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

<img width="1000" height="724" alt="image" src="https://github.com/user-attachments/assets/186c6c11-bfb0-473b-aa14-05673d6a79ab" />
<img width="907" height="736" alt="image" src="https://github.com/user-attachments/assets/ffad23ee-f39a-430a-82f9-32470d765b9b" />

Pie Chart:
```
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

<img width="859" height="734" alt="image" src="https://github.com/user-attachments/assets/8b186210-64a7-4543-973d-97665f5fa59f" />
<img width="935" height="741" alt="image" src="https://github.com/user-attachments/assets/2648c966-fb09-4057-b4ce-010a6ff960db" />

Area Chart:
```
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

<img width="1004" height="730" alt="image" src="https://github.com/user-attachments/assets/e2f8746f-f0ba-477e-a2a5-5d713a5dca85" />

Bar Chart:
```
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

<img width="922" height="731" alt="image" src="https://github.com/user-attachments/assets/1157bd67-1031-429a-b8f0-db11ae659e94" />

Histogram:
```
x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x, bins = 10, color='blue', alpha=0.5)
plt.show()
```

<img width="955" height="732" alt="image" src="https://github.com/user-attachments/assets/62824f17-bd03-46eb-ab15-542e5e367f80" />

Box Plot:
```
np.random.seed(0)
data=np.random.normal(loc=0, scale=1, size=100)
data
```

<img width="1181" height="733" alt="image" src="https://github.com/user-attachments/assets/2769af16-a9a0-4dd8-84bf-a93a59220895" />

```
fig, ax= plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```

<img width="869" height="735" alt="image" src="https://github.com/user-attachments/assets/1d79d928-c028-4703-9f2b-848edbe2a802" />

# Result:
 Thus, all the data visualization techniques of matplotlib has been implemented.
