# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY
```
    Name:Sanjay s
    Reg No: 212224110047
```
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
LINE GRAPHS

    import matplotlib.pyplot as plt
    x1 = [1, 2, 3, 8, 9]
    y1 = [4, 1, 3, 20, 18]
    plt.plot(x1, y1, marker='o', linestyle='-', color='b')
    plt.title("Simple Line Plot")
    plt.xlabel("X-axis")
    plt.ylabel("Y-axis")
    plt.grid(True)
    plt.show()
![image](https://github.com/user-attachments/assets/04293d5d-5399-4fff-b2f5-4f9a6a913e24)

    import matplotlib.pyplot as plt
    x1=[1,2,3]
    y1=[2,4,1]
    plt.plot(x1,y1,label="line 1",linewidth=6)
    x2=[1,2,3]
    y2=[4,1,3]
    plt.plot(x2,y2,label="line 2",linewidth=6)
    plt.xlabel('X-AXIS')
    plt.ylabel('Y-AXIS')
    plt.title("Two lines on the same graph")
    plt.legend()
![image](https://github.com/user-attachments/assets/9d8d208d-9c04-43d7-b2a7-50d682c5acd3)

    import matplotlib.pyplot as plt
    x=[1,2,3,4,5,6]
    y=[2,4,1,5,2,6]
    plt.plot(x,y,color='blue',linestyle='dashed',linewidth=4,marker='o',markerfacecolor='red',markersize=14)
    plt.ylim(1,8)
    plt.xlim(1,8)
    plt.xlabel('X-axis')
    plt.ylabel('Y-axis')
    plt.title('Some Cool Customizations')
![image](https://github.com/user-attachments/assets/0a9ca4f8-92f7-43b4-aad0-8add07522ed8)

Implementation using Matplotlib: Examples

    yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
    plt.plot(yield_apples)
![image](https://github.com/user-attachments/assets/de0fd8c0-b964-4965-a69e-67ec412b6e02)

    years=[2010,2011,2012,2013,2014,2015]
    yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
    plt.plot(years,yield_apples)
![image](https://github.com/user-attachments/assets/11492c4e-b046-40e7-9192-59d0ed8ff7c8)

    years=range(2000,2012)
    apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
    oranges=[0.962,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896,]
    plt.plot(years,apples,color='red',linewidth=5)
    plt.plot(years,oranges,color='orange',linewidth=5)
    plt.xlabel('YEAR')
    plt.ylabel('Yields (tons per hectare)')
    plt.title('Crop Yields in Kanto')
    plt.legend(['Apples','Oranges'])
![image](https://github.com/user-attachments/assets/ecd600b4-c400-4e4e-91f5-72dd053722ff)

    years=range(2000,2012)
    apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
    grapes=[0.926,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896, ]
    plt.plot(years, apples)
    plt.plot(years, grapes)
    plt.xlabel('Year')
    plt.ylabel('Yield (tons per hectare)')
    plt.title('Crop Yields')
    plt.legend(['Apples','grapes']);
![image](https://github.com/user-attachments/assets/e9e20b33-ac48-4699-8a25-5b8c71b328b9)

    plt.figure(figsize=(14,6))
    plt.plot(years,grapes,marker='o')
    plt.title("Yield of grapes (tons per hectare)");
![image](https://github.com/user-attachments/assets/1583f493-cd14-4c6b-94f3-a28c6092a757)

    plt.plot(years, apples, marker='o')
    plt.plot(years, oranges, marker='x')
    plt.xlabel('Year')
    plt.ylabel('Yield (tons per hectare)')
    plt.title("Crop Yields in Kanto")
    plt.legend(['Apples', 'Oranges'])
![image](https://github.com/user-attachments/assets/f8fc30b4-f1f7-4400-8706-e2b049aef041)

SCATTER PLOTS

    import matplotlib.pyplot as plt
    x_values=[0,1,2,3,4,5]
    y_values=[0,1,4,9,16,25]
    plt.scatter(x_values,y_values,s=100,c='purple')
    plt.xlabel('X-AXIS')
    plt.ylabel('Y-AXIS')
    plt.title('Scatter Plot')
![image](https://github.com/user-attachments/assets/08c003a0-4e03-4011-a2e3-e29cd8069569)

    import matplotlib.pyplot as plt
    x_values=[1,2,3,4,5,6,7,8,9,10]
    y_values=[2,4,5,7,6,8,9,11,12,12]
    plt.scatter(x_values,y_values,label='stars',marker='*',s=300,c='blue')
    plt.xlabel('X-AXIS')
    plt.ylabel('Y-AXIS')
    plt.title('Scatter Plot (Star)')
    plt.legend()
    plt.savefig("StarScatter.png")
![image](https://github.com/user-attachments/assets/f07553a7-51fa-442a-b0d4-d9d602a678ca)

    import matplotlib.pyplot as plt
    x=[1,2,3,4,5,6,7,8,9]
    y=[1,4,9,16,25,36,49,64,81]
    plt.xlabel('X-AXIS')
    plt.ylabel('Y-AXIS')
    plt.title('Scatter Plot Star')
    plt.subplot(2,2,1)
    plt.plot(x,y,'ro--')
    plt.subplot(2,2,2)
    plt.plot(y,x,'g*--')
    plt.subplot(2,2,3)
    plt.plot(x,x,'bo')
    plt.subplot(2,2,4)
    plt.plot(y,y,'go')
![image](https://github.com/user-attachments/assets/426c6ca5-a3d9-4c11-ac96-26eb1f44cbb5)

    plt.scatter(x,y,c='b')
    plt.xlabel('X-axis')
    plt.ylabel('Y-axis')
    plt.title('Graph in 2D')
    plt.savefig('Test.png')
![image](https://github.com/user-attachments/assets/a58f4603-a5b3-495b-9b1a-ae35a5c514b7)

    plt.plot(x,y,'y*',linestyle='dashed',color='cyan',linewidth=2,markersize=12)
    plt.xlabel('X axis')
    plt.ylabel('Y axis')
    plt.title('2d Diagram')
![image](https://github.com/user-attachments/assets/eb60788b-71f9-4ccf-8e59-4d243f9225a9)

    x=np.arange(0,4*np.pi,0.1)
    y=np.sin(x)
    plt.title("sine wave form")
    plt.plot(x,y)
    plt.show()
![image](https://github.com/user-attachments/assets/08af843d-3070-402a-88be-d829a07c99f2)

AREA CHART

    import matplotlib.pyplot as plt
    import numpy as np
    x=[1,2,3,4,5]
    y1=[10,12,14,16,18]
    y2=[5,7,9,11,13]
    y3=[2,4,6,8,10]
    plt.fill_between(x,y1,color='purple')
    plt.fill_between(x,y2,color='pink')
    plt.plot(x,y1,color='black')
    plt.plot(x,y2,color='white')
    plt.legend(['y1','y2'])
    plt.show()
![image](https://github.com/user-attachments/assets/546efc15-6964-4003-a04b-cee8cc560c40)

BAR CHART
    
    import matplotlib.pyplot as plt
    height = [10,24,36,40,5]
    names=['One','Two','Three','Four','Five']
    c1=['g','b']
    plt.bar(names,height,width=0.8,color=c1)
    plt.xlabel('X-AXIS')
    plt.ylabel('Y-AXIS')
    plt.title('Bar Graph')
![image](https://github.com/user-attachments/assets/02e6ae64-916a-4d72-a9a3-5d9e1cd67af4)

    x=[2,8,10]
    y=[11,16,9]
    x2=[3,9,11]
    y2=[6,15,7]
    plt.bar(x,y,color='r')
    plt.bar(x2,y2,color='b')
    plt.xlabel('X-AXIS')
    plt.ylabel('Y-AXIS')
    plt.title('Bar Graph')
![image](https://github.com/user-attachments/assets/a70dfb8c-1bc0-42c8-b000-c12a67e38c85)

HISTOGRAM

    import matplotlib.pyplot as plt
    ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
    range=(0,100)
    bins=10
    plt.hist(ages,bins,range,color='brown',histtype='bar',rwidth=0.8)
    plt.xlabel('age')
    plt.ylabel('no.of people')
    plt.title('Histogram')
![image](https://github.com/user-attachments/assets/26126847-bc0c-488b-be86-5cb87a39c35d)

    import matplotlib.pyplot as plt
    x=[2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
    plt.hist(x,bins=10,color='grey',alpha=0.5)
    plt.show()
![image](https://github.com/user-attachments/assets/3d3b5075-03fe-4bb8-965a-be61b6a425a2)

BOX PLOT

    import matplotlib.pyplot as plt
    import numpy as np
    np.random.seed(0)
    data=np.random.normal(loc=0,scale=1,size=100)
    data
![image](https://github.com/user-attachments/assets/e88b0fed-c040-474c-91d2-8e02629e1051)

    fig,ax=plt.subplots()
    ax.boxplot(data)
    ax.set_xlabel('Data')
    ax.set_ylabel('Values')
    ax.set_title('Box Plot')
![image](https://github.com/user-attachments/assets/ad8752a7-6dff-44fb-99b5-48328f6d3904)

PIE CHART

    labels='Python','C++','Ruby','Java'
    sizes=[215,130,245,210]
    colors=['gold','yellowgreen','lightcoral','lightskyblue']
    explode=(0,0.4,0,0.5)
    plt.pie(sizes,explode=explode,labels=labels,colors=colors,autopct='%1.1f%%',shadow=True)
    plt.axis('equal')
    plt.show()
![image](https://github.com/user-attachments/assets/79e2bba6-3ff2-4b35-89da-cd61053332a7)

    activities=['eat','sleep','work','play']
    slices=[3,7,8,6]
    colors=['r','y','g','b']
    plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
    plt.legend()
![image](https://github.com/user-attachments/assets/2d81cdaa-84d8-40f0-adc0-2cbf0b337be0)

# Result:
Thus, The implementation of data visualization using matplotlib has been successfully verified.
