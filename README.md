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
~~~
import matplotlib.pyplot as plt

%matplotlib inline

import numpy as np

## Simple Examples

x=np.arange(0,10)
y=np.arange(11,21)

a=np.arange(40,50)
b=np.arange(50,60)

##plotting using matplotlib 

##plt scatter

plt.scatter(x,y,c='g')
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')

y=x*x

## plt plot

plt.plot(x,y,'r*',linestyle='dashed',linewidth=2, markersize=12)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')
plt.show()

## Creating Subplots

plt.subplot(2,2,1)
plt.plot(x,y,'r--')
plt.subplot(2,2,2)
plt.plot(x,y,'g*--')
plt.subplot(2,2,3)
plt.plot(x,y,'bo')
plt.subplot(2,2,4)
plt.plot(x,y,'go')
plt.show()

x = np.arange(1,11) 
y = 3 * x + 5 
plt.title("Matplotlib demo") 
plt.xlabel("x axis caption") 
plt.ylabel("y axis caption") 
plt.plot(x,y) 
plt.show()

np.pi

# Compute the x and y coordinates for points on a sine curve 
x = np.arange(0, 4 * np.pi, 0.1) 
y = np.sin(x) 
plt.title("sine wave form") 

# Plot the points using matplotlib 
plt.plot(x, y) 
plt.show() 

#Subplot()
# Compute the x and y coordinates for points on sine and cosine curves 
x = np.arange(0, 5 * np.pi, 0.1) 
y_sin = np.sin(x) 
y_cos = np.cos(x)  
   
# Set up a subplot grid that has height 2 and width 1, 
# and set the first such subplot as active. 
plt.subplot(2, 1, 1)
   
# Make the first plot 
plt.plot(x, y_sin,'r--') 
plt.title('Sine')  
   
# Set the second subplot as active, and make the second plot. 
plt.subplot(2, 1, 2) 
plt.plot(x, y_cos,'g--') 
plt.title('Cosine')  
   
# Show the figure. 
plt.show()

#Subplot()
# Compute the x and y coordinates for points on sine and cosine curves 
x = np.arange(0, 5 * np.pi, 0.1) 
y_sin = np.sin(x) 
y_cos = np.cos(x)  
   
# Set up a subplot grid that has height 2 and width 1, 
# and set the first such subplot as active. 
plt.subplot(2, 1, 1)
   
# Make the first plot 
plt.plot(x, y_sin,'r--') 
plt.title('Sine')  
   
# Set the second subplot as active, and make the second plot. 
plt.subplot(2, 1, 2) 
plt.plot(x, y_cos,'g--') 
plt.title('Cosine')  
   
# Show the figure. 
plt.show()

## Bar plot

x = [2,8,10] 
y = [11,16,9]  

x2 = [3,9,11] 
y2 = [6,15,7] 
plt.bar(x, y) 
plt.bar(x2, y2, color = 'g') 
plt.title('Bar graph') 
plt.ylabel('Y axis') 
plt.xlabel('X axis')  

plt.show()

a = np.array([22,87,5,43,56,73,55,54,11,20,51,5,79,31,27]) 
plt.hist(a) 
plt.title("histogram") 
plt.show()

data = [np.random.normal(0, std, 100) for std in range(1, 4)]

# rectangular box plot
plt.boxplot(data,vert=True,patch_artist=False);  
plt.show()

data = [np.random.normal(0, std, 100) for std in range(1, 4)]

# rectangular box plot
plt.boxplot(data,vert=True,patch_artist=True);
plt.show() 

data

# Data to plot
labels = 'sepal_length', 'sepal_width', 'petal_length', 'petal_width'
sizes = [215, 130, 245, 210]
colors = ['gold', 'yellowgreen', 'lightcoral', 'lightskyblue']
explode = (0.4, 0, 0, 0)  # explode 1st slice

# Plot
plt.pie(sizes, explode=explode, labels=labels, colors=colors,
autopct='%1.1f%%', shadow=False)

plt.axis('equal')
plt.show()
~~~
<img width="843" height="683" alt="image" src="https://github.com/user-attachments/assets/d66968f5-003d-429a-811f-04840b08514b" />
<img width="848" height="684" alt="image" src="https://github.com/user-attachments/assets/5ae68696-6df4-4eb2-bab8-03a82acb16b8" />
<img width="848" height="687" alt="image" src="https://github.com/user-attachments/assets/037fa67a-1a21-4084-920a-9b6dc09f9a62" />
<img width="818" height="645" alt="image" src="https://github.com/user-attachments/assets/a90157eb-0fc2-4faa-b4d7-ca7b30e24b0c" />
<img width="818" height="621" alt="image" src="https://github.com/user-attachments/assets/b9022c1f-6249-42d3-afab-93c05ee31918" />
<img width="772" height="584" alt="image" src="https://github.com/user-attachments/assets/0f92e629-9a6f-41e5-894b-d9c61cf7b055" />

# Result:
Thus, the Data Visualization using matplot python library is successfully performed.
