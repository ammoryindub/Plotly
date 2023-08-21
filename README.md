# Plotly


The 'dataset.csv' file is associated with 01-Plotly-Cufflinks

The '2012_Election_Data', '2014_World_Power_Consumption' files are associated with 01-Plotly-Maps.


#### Plotly & Cufflinks

- installing Plotly, cufflinks, chart-studio libraries

- Import libraries

- Importing data

- 



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

box plot

3D surface plot

histogram plot

spread




bubble plot

scatter matrix

