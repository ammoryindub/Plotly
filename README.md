# Plotly


The 'dataset.csv' file is associated with 01-Plotly-Cufflinks

The '2012_Election_Data', '2014_World_Power_Consumption' files are associated with 01-Plotly-Maps.


Plotly & Cufflinks
Plotly is a library that allows you to create interactive plots, you can use in dashboards or websites.

N: You can save them as html files or static images
#installing plotly library

!pip install plotly 
Requirement already satisfied: plotly in /Users/alex/anaconda3/lib/python3.10/site-packages (5.9.0)
Requirement already satisfied: tenacity>=6.2.0 in /Users/alex/anaconda3/lib/python3.10/site-packages (from plotly) (8.0.1)
# installing cufflinks library

!pip install cufflinks
Collecting cufflinks
  Downloading cufflinks-0.17.3.tar.gz (81 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 81.7/81.7 kB 796.5 kB/s eta 0:00:00a 0:00:01
  Preparing metadata (setup.py) ... done
Requirement already satisfied: numpy>=1.9.2 in /Users/alex/anaconda3/lib/python3.10/site-packages (from cufflinks) (1.23.5)
Requirement already satisfied: pandas>=0.19.2 in /Users/alex/anaconda3/lib/python3.10/site-packages (from cufflinks) (1.5.3)
Requirement already satisfied: plotly>=4.1.1 in /Users/alex/anaconda3/lib/python3.10/site-packages (from cufflinks) (5.9.0)
Requirement already satisfied: six>=1.9.0 in /Users/alex/anaconda3/lib/python3.10/site-packages (from cufflinks) (1.16.0)
Collecting colorlover>=0.2.1
  Downloading colorlover-0.3.0-py3-none-any.whl (8.9 kB)
Requirement already satisfied: setuptools>=34.4.1 in /Users/alex/anaconda3/lib/python3.10/site-packages (from cufflinks) (65.6.3)
Requirement already satisfied: ipython>=5.3.0 in /Users/alex/anaconda3/lib/python3.10/site-packages (from cufflinks) (8.10.0)
Requirement already satisfied: ipywidgets>=7.0.0 in /Users/alex/anaconda3/lib/python3.10/site-packages (from cufflinks) (7.6.5)
Requirement already satisfied: backcall in /Users/alex/anaconda3/lib/python3.10/site-packages (from ipython>=5.3.0->cufflinks) (0.2.0)
Requirement already satisfied: appnope in /Users/alex/anaconda3/lib/python3.10/site-packages (from ipython>=5.3.0->cufflinks) (0.1.2)
Requirement already satisfied: matplotlib-inline in /Users/alex/anaconda3/lib/python3.10/site-packages (from ipython>=5.3.0->cufflinks) (0.1.6)
Requirement already satisfied: pickleshare in /Users/alex/anaconda3/lib/python3.10/site-packages (from ipython>=5.3.0->cufflinks) (0.7.5)
Requirement already satisfied: jedi>=0.16 in /Users/alex/anaconda3/lib/python3.10/site-packages (from ipython>=5.3.0->cufflinks) (0.18.1)
Requirement already satisfied: decorator in /Users/alex/anaconda3/lib/python3.10/site-packages (from ipython>=5.3.0->cufflinks) (5.1.1)
Requirement already satisfied: pygments>=2.4.0 in /Users/alex/anaconda3/lib/python3.10/site-packages (from ipython>=5.3.0->cufflinks) (2.11.2)
Requirement already satisfied: traitlets>=5 in /Users/alex/anaconda3/lib/python3.10/site-packages (from ipython>=5.3.0->cufflinks) (5.7.1)
Requirement already satisfied: pexpect>4.3 in /Users/alex/anaconda3/lib/python3.10/site-packages (from ipython>=5.3.0->cufflinks) (4.8.0)
Requirement already satisfied: prompt-toolkit<3.1.0,>=3.0.30 in /Users/alex/anaconda3/lib/python3.10/site-packages (from ipython>=5.3.0->cufflinks) (3.0.36)
Requirement already satisfied: stack-data in /Users/alex/anaconda3/lib/python3.10/site-packages (from ipython>=5.3.0->cufflinks) (0.2.0)
Requirement already satisfied: jupyterlab-widgets>=1.0.0 in /Users/alex/anaconda3/lib/python3.10/site-packages (from ipywidgets>=7.0.0->cufflinks) (1.0.0)
Requirement already satisfied: nbformat>=4.2.0 in /Users/alex/anaconda3/lib/python3.10/site-packages (from ipywidgets>=7.0.0->cufflinks) (5.7.0)
Requirement already satisfied: ipython-genutils~=0.2.0 in /Users/alex/anaconda3/lib/python3.10/site-packages (from ipywidgets>=7.0.0->cufflinks) (0.2.0)
Requirement already satisfied: widgetsnbextension~=3.5.0 in /Users/alex/anaconda3/lib/python3.10/site-packages (from ipywidgets>=7.0.0->cufflinks) (3.5.2)
Requirement already satisfied: ipykernel>=4.5.1 in /Users/alex/anaconda3/lib/python3.10/site-packages (from ipywidgets>=7.0.0->cufflinks) (6.19.2)
Requirement already satisfied: python-dateutil>=2.8.1 in /Users/alex/anaconda3/lib/python3.10/site-packages (from pandas>=0.19.2->cufflinks) (2.8.2)
Requirement already satisfied: pytz>=2020.1 in /Users/alex/anaconda3/lib/python3.10/site-packages (from pandas>=0.19.2->cufflinks) (2022.7)
Requirement already satisfied: tenacity>=6.2.0 in /Users/alex/anaconda3/lib/python3.10/site-packages (from plotly>=4.1.1->cufflinks) (8.0.1)
Requirement already satisfied: nest-asyncio in /Users/alex/anaconda3/lib/python3.10/site-packages (from ipykernel>=4.5.1->ipywidgets>=7.0.0->cufflinks) (1.5.6)
Requirement already satisfied: psutil in /Users/alex/anaconda3/lib/python3.10/site-packages (from ipykernel>=4.5.1->ipywidgets>=7.0.0->cufflinks) (5.9.0)
Requirement already satisfied: comm>=0.1.1 in /Users/alex/anaconda3/lib/python3.10/site-packages (from ipykernel>=4.5.1->ipywidgets>=7.0.0->cufflinks) (0.1.2)
Requirement already satisfied: packaging in /Users/alex/anaconda3/lib/python3.10/site-packages (from ipykernel>=4.5.1->ipywidgets>=7.0.0->cufflinks) (22.0)
Requirement already satisfied: tornado>=6.1 in /Users/alex/anaconda3/lib/python3.10/site-packages (from ipykernel>=4.5.1->ipywidgets>=7.0.0->cufflinks) (6.1)
Requirement already satisfied: debugpy>=1.0 in /Users/alex/anaconda3/lib/python3.10/site-packages (from ipykernel>=4.5.1->ipywidgets>=7.0.0->cufflinks) (1.5.1)
Requirement already satisfied: jupyter-client>=6.1.12 in /Users/alex/anaconda3/lib/python3.10/site-packages (from ipykernel>=4.5.1->ipywidgets>=7.0.0->cufflinks) (7.3.4)
Requirement already satisfied: pyzmq>=17 in /Users/alex/anaconda3/lib/python3.10/site-packages (from ipykernel>=4.5.1->ipywidgets>=7.0.0->cufflinks) (23.2.0)
Requirement already satisfied: parso<0.9.0,>=0.8.0 in /Users/alex/anaconda3/lib/python3.10/site-packages (from jedi>=0.16->ipython>=5.3.0->cufflinks) (0.8.3)
Requirement already satisfied: jsonschema>=2.6 in /Users/alex/anaconda3/lib/python3.10/site-packages (from nbformat>=4.2.0->ipywidgets>=7.0.0->cufflinks) (4.17.3)
Requirement already satisfied: fastjsonschema in /Users/alex/anaconda3/lib/python3.10/site-packages (from nbformat>=4.2.0->ipywidgets>=7.0.0->cufflinks) (2.16.2)
Requirement already satisfied: jupyter-core in /Users/alex/anaconda3/lib/python3.10/site-packages (from nbformat>=4.2.0->ipywidgets>=7.0.0->cufflinks) (5.2.0)
Requirement already satisfied: ptyprocess>=0.5 in /Users/alex/anaconda3/lib/python3.10/site-packages (from pexpect>4.3->ipython>=5.3.0->cufflinks) (0.7.0)
Requirement already satisfied: wcwidth in /Users/alex/anaconda3/lib/python3.10/site-packages (from prompt-toolkit<3.1.0,>=3.0.30->ipython>=5.3.0->cufflinks) (0.2.5)
Requirement already satisfied: notebook>=4.4.1 in /Users/alex/anaconda3/lib/python3.10/site-packages (from widgetsnbextension~=3.5.0->ipywidgets>=7.0.0->cufflinks) (6.5.2)
Requirement already satisfied: executing in /Users/alex/anaconda3/lib/python3.10/site-packages (from stack-data->ipython>=5.3.0->cufflinks) (0.8.3)
Requirement already satisfied: asttokens in /Users/alex/anaconda3/lib/python3.10/site-packages (from stack-data->ipython>=5.3.0->cufflinks) (2.0.5)
Requirement already satisfied: pure-eval in /Users/alex/anaconda3/lib/python3.10/site-packages (from stack-data->ipython>=5.3.0->cufflinks) (0.2.2)
Requirement already satisfied: attrs>=17.4.0 in /Users/alex/anaconda3/lib/python3.10/site-packages (from jsonschema>=2.6->nbformat>=4.2.0->ipywidgets>=7.0.0->cufflinks) (22.1.0)
Requirement already satisfied: pyrsistent!=0.17.0,!=0.17.1,!=0.17.2,>=0.14.0 in /Users/alex/anaconda3/lib/python3.10/site-packages (from jsonschema>=2.6->nbformat>=4.2.0->ipywidgets>=7.0.0->cufflinks) (0.18.0)
Requirement already satisfied: entrypoints in /Users/alex/anaconda3/lib/python3.10/site-packages (from jupyter-client>=6.1.12->ipykernel>=4.5.1->ipywidgets>=7.0.0->cufflinks) (0.4)
Requirement already satisfied: platformdirs>=2.5 in /Users/alex/anaconda3/lib/python3.10/site-packages (from jupyter-core->nbformat>=4.2.0->ipywidgets>=7.0.0->cufflinks) (2.5.2)
Requirement already satisfied: argon2-cffi in /Users/alex/anaconda3/lib/python3.10/site-packages (from notebook>=4.4.1->widgetsnbextension~=3.5.0->ipywidgets>=7.0.0->cufflinks) (21.3.0)
Requirement already satisfied: Send2Trash>=1.8.0 in /Users/alex/anaconda3/lib/python3.10/site-packages (from notebook>=4.4.1->widgetsnbextension~=3.5.0->ipywidgets>=7.0.0->cufflinks) (1.8.0)
Requirement already satisfied: prometheus-client in /Users/alex/anaconda3/lib/python3.10/site-packages (from notebook>=4.4.1->widgetsnbextension~=3.5.0->ipywidgets>=7.0.0->cufflinks) (0.14.1)
Requirement already satisfied: jinja2 in /Users/alex/anaconda3/lib/python3.10/site-packages (from notebook>=4.4.1->widgetsnbextension~=3.5.0->ipywidgets>=7.0.0->cufflinks) (3.1.2)
Requirement already satisfied: terminado>=0.8.3 in /Users/alex/anaconda3/lib/python3.10/site-packages (from notebook>=4.4.1->widgetsnbextension~=3.5.0->ipywidgets>=7.0.0->cufflinks) (0.17.1)
Requirement already satisfied: nbconvert>=5 in /Users/alex/anaconda3/lib/python3.10/site-packages (from notebook>=4.4.1->widgetsnbextension~=3.5.0->ipywidgets>=7.0.0->cufflinks) (6.5.4)
Requirement already satisfied: nbclassic>=0.4.7 in /Users/alex/anaconda3/lib/python3.10/site-packages (from notebook>=4.4.1->widgetsnbextension~=3.5.0->ipywidgets>=7.0.0->cufflinks) (0.5.2)
Requirement already satisfied: notebook-shim>=0.1.0 in /Users/alex/anaconda3/lib/python3.10/site-packages (from nbclassic>=0.4.7->notebook>=4.4.1->widgetsnbextension~=3.5.0->ipywidgets>=7.0.0->cufflinks) (0.2.2)
Requirement already satisfied: jupyter-server>=1.8 in /Users/alex/anaconda3/lib/python3.10/site-packages (from nbclassic>=0.4.7->notebook>=4.4.1->widgetsnbextension~=3.5.0->ipywidgets>=7.0.0->cufflinks) (1.23.4)
Requirement already satisfied: defusedxml in /Users/alex/anaconda3/lib/python3.10/site-packages (from nbconvert>=5->notebook>=4.4.1->widgetsnbextension~=3.5.0->ipywidgets>=7.0.0->cufflinks) (0.7.1)
Requirement already satisfied: bleach in /Users/alex/anaconda3/lib/python3.10/site-packages (from nbconvert>=5->notebook>=4.4.1->widgetsnbextension~=3.5.0->ipywidgets>=7.0.0->cufflinks) (4.1.0)
Requirement already satisfied: nbclient>=0.5.0 in /Users/alex/anaconda3/lib/python3.10/site-packages (from nbconvert>=5->notebook>=4.4.1->widgetsnbextension~=3.5.0->ipywidgets>=7.0.0->cufflinks) (0.5.13)
Requirement already satisfied: pandocfilters>=1.4.1 in /Users/alex/anaconda3/lib/python3.10/site-packages (from nbconvert>=5->notebook>=4.4.1->widgetsnbextension~=3.5.0->ipywidgets>=7.0.0->cufflinks) (1.5.0)
Requirement already satisfied: tinycss2 in /Users/alex/anaconda3/lib/python3.10/site-packages (from nbconvert>=5->notebook>=4.4.1->widgetsnbextension~=3.5.0->ipywidgets>=7.0.0->cufflinks) (1.2.1)
Requirement already satisfied: mistune<2,>=0.8.1 in /Users/alex/anaconda3/lib/python3.10/site-packages (from nbconvert>=5->notebook>=4.4.1->widgetsnbextension~=3.5.0->ipywidgets>=7.0.0->cufflinks) (0.8.4)
Requirement already satisfied: jupyterlab-pygments in /Users/alex/anaconda3/lib/python3.10/site-packages (from nbconvert>=5->notebook>=4.4.1->widgetsnbextension~=3.5.0->ipywidgets>=7.0.0->cufflinks) (0.1.2)
Requirement already satisfied: lxml in /Users/alex/anaconda3/lib/python3.10/site-packages (from nbconvert>=5->notebook>=4.4.1->widgetsnbextension~=3.5.0->ipywidgets>=7.0.0->cufflinks) (4.9.1)
Requirement already satisfied: MarkupSafe>=2.0 in /Users/alex/anaconda3/lib/python3.10/site-packages (from nbconvert>=5->notebook>=4.4.1->widgetsnbextension~=3.5.0->ipywidgets>=7.0.0->cufflinks) (2.1.1)
Requirement already satisfied: beautifulsoup4 in /Users/alex/anaconda3/lib/python3.10/site-packages (from nbconvert>=5->notebook>=4.4.1->widgetsnbextension~=3.5.0->ipywidgets>=7.0.0->cufflinks) (4.11.1)
Requirement already satisfied: argon2-cffi-bindings in /Users/alex/anaconda3/lib/python3.10/site-packages (from argon2-cffi->notebook>=4.4.1->widgetsnbextension~=3.5.0->ipywidgets>=7.0.0->cufflinks) (21.2.0)
Requirement already satisfied: anyio<4,>=3.1.0 in /Users/alex/anaconda3/lib/python3.10/site-packages (from jupyter-server>=1.8->nbclassic>=0.4.7->notebook>=4.4.1->widgetsnbextension~=3.5.0->ipywidgets>=7.0.0->cufflinks) (3.5.0)
Requirement already satisfied: websocket-client in /Users/alex/anaconda3/lib/python3.10/site-packages (from jupyter-server>=1.8->nbclassic>=0.4.7->notebook>=4.4.1->widgetsnbextension~=3.5.0->ipywidgets>=7.0.0->cufflinks) (0.58.0)
Requirement already satisfied: cffi>=1.0.1 in /Users/alex/anaconda3/lib/python3.10/site-packages (from argon2-cffi-bindings->argon2-cffi->notebook>=4.4.1->widgetsnbextension~=3.5.0->ipywidgets>=7.0.0->cufflinks) (1.15.1)
Requirement already satisfied: soupsieve>1.2 in /Users/alex/anaconda3/lib/python3.10/site-packages (from beautifulsoup4->nbconvert>=5->notebook>=4.4.1->widgetsnbextension~=3.5.0->ipywidgets>=7.0.0->cufflinks) (2.3.2.post1)
Requirement already satisfied: webencodings in /Users/alex/anaconda3/lib/python3.10/site-packages (from bleach->nbconvert>=5->notebook>=4.4.1->widgetsnbextension~=3.5.0->ipywidgets>=7.0.0->cufflinks) (0.5.1)
Requirement already satisfied: idna>=2.8 in /Users/alex/anaconda3/lib/python3.10/site-packages (from anyio<4,>=3.1.0->jupyter-server>=1.8->nbclassic>=0.4.7->notebook>=4.4.1->widgetsnbextension~=3.5.0->ipywidgets>=7.0.0->cufflinks) (3.4)
Requirement already satisfied: sniffio>=1.1 in /Users/alex/anaconda3/lib/python3.10/site-packages (from anyio<4,>=3.1.0->jupyter-server>=1.8->nbclassic>=0.4.7->notebook>=4.4.1->widgetsnbextension~=3.5.0->ipywidgets>=7.0.0->cufflinks) (1.2.0)
Requirement already satisfied: pycparser in /Users/alex/anaconda3/lib/python3.10/site-packages (from cffi>=1.0.1->argon2-cffi-bindings->argon2-cffi->notebook>=4.4.1->widgetsnbextension~=3.5.0->ipywidgets>=7.0.0->cufflinks) (2.21)
Building wheels for collected packages: cufflinks
  Building wheel for cufflinks (setup.py) ... done
  Created wheel for cufflinks: filename=cufflinks-0.17.3-py3-none-any.whl size=67902 sha256=439708b9dfc92ed2d2d025df99b0a2549500b754fb90264ec72bc18a369c0efa
  Stored in directory: /Users/alex/Library/Caches/pip/wheels/b1/8f/ec/b76ac80a14f3f5f59643cbc2eee7d78690b1bd158279f299dd
Successfully built cufflinks
Installing collected packages: colorlover, cufflinks
Successfully installed colorlover-0.3.0 cufflinks-0.17.3
# installing chart-studio library

!pip install chart-studio
Collecting chart-studio
  Downloading chart_studio-1.1.0-py3-none-any.whl (64 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 64.4/64.4 kB 724.7 kB/s eta 0:00:00a 0:00:01
Requirement already satisfied: plotly in /Users/alex/anaconda3/lib/python3.10/site-packages (from chart-studio) (5.9.0)
Requirement already satisfied: six in /Users/alex/anaconda3/lib/python3.10/site-packages (from chart-studio) (1.16.0)
Collecting retrying>=1.3.3
  Downloading retrying-1.3.4-py3-none-any.whl (11 kB)
Requirement already satisfied: requests in /Users/alex/anaconda3/lib/python3.10/site-packages (from chart-studio) (2.28.1)
Requirement already satisfied: tenacity>=6.2.0 in /Users/alex/anaconda3/lib/python3.10/site-packages (from plotly->chart-studio) (8.0.1)
Requirement already satisfied: charset-normalizer<3,>=2 in /Users/alex/anaconda3/lib/python3.10/site-packages (from requests->chart-studio) (2.0.4)
Requirement already satisfied: certifi>=2017.4.17 in /Users/alex/anaconda3/lib/python3.10/site-packages (from requests->chart-studio) (2023.5.7)
Requirement already satisfied: idna<4,>=2.5 in /Users/alex/anaconda3/lib/python3.10/site-packages (from requests->chart-studio) (3.4)
Requirement already satisfied: urllib3<1.27,>=1.21.1 in /Users/alex/anaconda3/lib/python3.10/site-packages (from requests->chart-studio) (1.26.14)
Installing collected packages: retrying, chart-studio
Successfully installed chart-studio-1.1.0 retrying-1.3.4
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

