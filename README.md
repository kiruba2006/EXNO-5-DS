# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Name:Kiruba RC
# REG NO:212224230125
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
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
```
```
x=[2018,2019, 2020,2021,2022]
y=[15000,20000,25000,30000,35000]
plt.plot(x,y, 'g*',linestyle='dashed', linewidth=2, markersize=12)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('2D Diagram')
plt.show()
```
<img width="852" height="582" alt="image" src="https://github.com/user-attachments/assets/b1222415-c419-4385-90bd-c2260997208d" />

```
plt.subplot(2,2,1)
plt.plot(x,y,'r--')
plt.subplot(2,2,2)
plt.plot(x,y, 'g--')
plt.subplot(2,2,3)
plt.plot(x,y, 'bo') 
plt.subplot(2,2,4)
plt.plot(x,y,'go')
```
<img width="745" height="555" alt="image" src="https://github.com/user-attachments/assets/3397603d-4333-414c-b0e2-e435bec39b58" />

```
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine waveform")
plt.plot(x,y)
plt.show()
```
<img width="796" height="562" alt="image" src="https://github.com/user-attachments/assets/aed2068d-5738-49fb-8d8b-2a0238cf61b2" />

```
x=[2,8,10]
y=[11,16,9]
x1=[3,9,11]
y1=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x1,y1,color='g')
plt.title("Bar graph")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```
<img width="768" height="576" alt="image" src="https://github.com/user-attachments/assets/a1cd5e48-f6d6-4d88-be64-85096141b117" />

```
x=[1,2,3]
y=[7,3,9]

plt.plot(x,y,color='g')
plt.title("line graph")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```
<img width="721" height="561" alt="image" src="https://github.com/user-attachments/assets/83283d82-7eee-4cf1-8153-fad0db7c2a4f" />

```
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1,label='line1')
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label='line2')
plt.title("multiple graph")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.legend()
plt.show()
```
<img width="752" height="582" alt="image" src="https://github.com/user-attachments/assets/5e542e7e-8a46-4281-8350-6de75b62d24c" />

```
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6] 
plt.plot(x,y,color='green', linestyle='dashed',linewidth=3,marker='o', markerfacecolor='red', markersize=12, label='spices')
plt.ylim(1,8)
plt.xlim(1,8)
plt.title("line graph")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.legend()
plt.show()
```
<img width="756" height="592" alt="image" src="https://github.com/user-attachments/assets/d1c102b5-eb3e-4206-91fc-3b6f429605e5" />

```
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples, linestyle='dashed',linewidth=3, marker='*',markersize=12,color='g')
plt.show()
```
<img width="778" height="517" alt="image" src="https://github.com/user-attachments/assets/c3439a2f-faca-408a-98d4-43303df15551" />

```
oranges=[2,4,6,7,8,12,45] apples=[2,4,5,6,8,23,37]
years=[2019,2020,2021,2022, 2023, 2024, 2025]
plt.plot(years, apples, marker='o')
plt.plot(years, oranges, marker='*')
plt.title("crop yields in kanto")
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')
plt.legend(['apples', 'oranges'])
plt.show))
```
<img width="772" height="575" alt="image" src="https://github.com/user-attachments/assets/5d2540c1-1d7d-4479-a364-52447939c757" />

```
oranges=[2,4,6,7,8,12]
apples=[2,4,5,6,8,23]
years=[2019,2020,2021,2022, 2023, 2024]
plt.bar(oranges, apples)
plt.plot(years, apples, label='apples', marker='*')
plt.plot(years, oranges, label='oranges', marker='o')
plt.title("Fruit sales")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.legend()
plt.show()
```
<img width="756" height="583" alt="image" src="https://github.com/user-attachments/assets/6ca24e8a-f861-46e3-bd0e-624c8440ac20" />

```
plt.figure(figsize=(12,6))
plt.plot(years,oranges, marker='o', label='oranges')
plt.title("Yield of oranges (tons per hectare)")
plt.legend()
```
<img width="761" height="445" alt="image" src="https://github.com/user-attachments/assets/50beb0da-7e3c-44d0-bffc-77a5e4079f20" />

```
print("scatter plot is:")
x=[1,2,3,4,5,6,7,8,9,10]
y=[2,4,5,7,6,8,9,11,12,12] 
plt.scatter(x,y, label='star', color='green', marker='*',s=30)
plt.title("my scatterplot!")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.legend()
plt.show()
```
<img width="772" height="592" alt="image" src="https://github.com/user-attachments/assets/12af010d-b288-4bb1-95a4-83947253046e" />

```
x=[1,2,3,4,5] 
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10] 
plt.fill_between(x,y1,color='green', label='y1')
plt.fill_between (x,y2, color='blue', label='y2')
plt.fill_between (x,y3, color='red', label='y3')
plt.title("fill between is")
plt.legend()
plt.show()
```
<img width="749" height="554" alt="image" src="https://github.com/user-attachments/assets/56364189-2942-4b63-957e-f64ced6ef87f" />


```
plt.stackplot(x,y1, y2,y3, labels=['linel', 'line2', 'line3'])
plt.legend(loc='upper left')
plt.title("Stacked line chart")
plt.xlabel('x-axis')
plt.ylabel('y-axis') 
plt.show()
```

<img width="741" height="566" alt="image" src="https://github.com/user-attachments/assets/25be5481-cc31-4a1f-9fc6-04ac20e5e358" />

```
from scipy.interpolate import make_interp_spline
x=np.array ([1,2,3,4,5,6,7,8,9,10])
y=np.array([2,4,5,7,8,9,10,11,12,13])
spl=make_interp_spline(x,y)
x_smooth=np.linspace(x.min(),x.max(),100)
y_smooth=spl(x_smooth)
plt.plot(x,y, 'o', label='data') 
plt.plot(x_smooth,y_smooth,'-', label='spline')
plt.legend()
plt.show()
```
<img width="728" height="527" alt="image" src="https://github.com/user-attachments/assets/ab1bcf4f-b277-4b64-aadc-7ef9d21de483" />

```
values=[5,6,7,3,2]
names=['A','B','C','D','E']
plt.bar(names,values,color='green')
plt.show()
```
<img width="714" height="529" alt="image" src="https://github.com/user-attachments/assets/65157d41-aebb-4f6e-9d7a-aa1ab116b4d7" />

```
ages=[2,5,70,40,45,50,43,40,44,60,7,13,57,18,90, 77, 32,21,20,40]
range1=(0,100)
bins=10
plt.hist(ages, bins, range1, color='green', histtype='bar', rwidth=0.8)
plt.xlabel('ages')
plt.ylabel('no.of people')
plt.title('my histogram')
plt.show
```
<img width="771" height="612" alt="image" src="https://github.com/user-attachments/assets/17c9b37c-c392-4382-8866-3f2d02e3f7a3" />

```
x=[2,1,6,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1] 
plt.hist(x,bins=10,color='green', alpha=0.5)
plt.show()
```
<img width="697" height="515" alt="image" src="https://github.com/user-attachments/assets/f8cec26f-b5fa-429b-85b7-3b26338db3bd" />

```
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```
<img width="721" height="439" alt="image" src="https://github.com/user-attachments/assets/a94e4b98-22c9-47f7-a904-5ccc8b5f30e3" />


```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('x-axis')
ax.set_ylabel('y-axis')
ax.set_title('box plot')
```
<img width="768" height="571" alt="image" src="https://github.com/user-attachments/assets/cc68c8d7-19e7-4992-b90e-f6f0d89573da" />

```
activities=['eat', 'sleep', 'work', 'play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices, labels=activities, colors=colors, startangle=90, shadow=True, explode=(0,0,0.1,0),radius=1.2, autopct="x1.1")
plt.legend()
plt.show()
```
<img width="673" height="519" alt="image" src="https://github.com/user-attachments/assets/5fe305b2-700e-4314-baad-e3c6766044ad" />

```
labels='python','c+','ruby','java'
sizes=[215,130,245,210]
colors=['gold', 'yellowgreen', 'lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode, colors=colors, labels=labels, autopct='%1.1f%%', shadow=True)
plt.axis('equal')
plt.show()
```
<img width="628" height="492" alt="image" src="https://github.com/user-attachments/assets/7301336e-6e55-49c4-80fc-559c1625e790" />





# Result:
Thus, The implementation of data visualization using matplotlib has been successfully verified.
