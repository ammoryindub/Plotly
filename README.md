# Plotly


The 'dataset.csv' file is associated with 01-Plotly-Cufflinks

The '2012_Election_Data', '2014_World_Power_Consumption' files are associated with 01-Plotly-Maps.


#### Plotly & Cufflinks

- installing Plotly, cufflinks libraries


# importing chart-studio plotly

import chart_studio.plotly as py
# importing usual libraries we need

import numpy as np
import pandas as pd 

%matplotlib inline
# importing library version and print it

from plotly import __version__

print(__version__)
5.9.0
import cufflinks as cf
# import from plotly, offline support because we will be suing its library offline

from plotly.offline import download_plotlyjs, init_notebook_mode, plot,iplot
# to make sure everyhting working in our notebook, it is going to connect JavaScript to our notebook

init_notebook_mode(connected =True)
# use go_offline() method it allows cufflinks to go offline 

cf.go_offline()
# we call our dataset

df1 = pd.read_csv('dataset.csv')
df1
a	b	c	d
0	0.336272	0.325011	0.001020	0.401402
1	0.980265	0.831835	0.772288	0.076485
2	0.480387	0.686839	0.000575	0.746758
3	0.502106	0.305142	0.768608	0.654685
4	0.856602	0.171448	0.157971	0.321231
...	...	...	...	...
495	0.528705	0.226122	0.055835	0.131962
496	0.324730	0.215201	0.935302	0.794115
497	0.118036	0.264574	0.629206	0.824062
498	0.227021	0.660209	0.851353	0.478676
499	0.466157	0.753000	0.115391	0.279712
500 rows × 4 columns

# we will establish random dataset we will be used later for barplot style.

df2 = pd.DataFrame ({'Category':['A','B','C'], 'Values':[34, 49, 56]})
df2
Category	Values
0	A	34
1	B	49
2	C	56
check the differnce of using plotly, by using two different methods ".plot()" and ".iplot()"
df1.plot(figsize=(14, 4))
<Axes: >

df1.iplot(size=(30, 4))

# you can notice the changes between both plots 
different types of plots
scatter plot
# using scatter plot between culomns a, b

df1.iplot(kind='scatter', x='a', y='b')
# scatter plot with arguments 

df1.iplot(kind='scatter', x='a', y='b', mode='markers',size=10, color = 'lightblue')
bar plot
# using df2

df2.iplot(kind='bar', x='Category', y='Values', 
          title='Bar Plot',
          xTitle='Category',
          yTitle='Values',
          barmode='group',   # Set the bar mode (group, stack, overlay)
          bargap=0.2,  # Set the gap between bars
          bargroupgap=0.1,  # Set the gap between bar groups
          showlegend=True,  # Show or hide the legend
         )
     
# using big data like df1, and use grouping methods  

df1.count().iplot(kind='bar')
df1.sum().iplot(kind='bar')
df1.mean().iplot(kind='bar')
box plot
df1.iplot(kind='box')
3D surface plot

histogram plot

spread




bubble plot

scatter matrix

