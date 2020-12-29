# Data analysis on FIFA 2020-21

# Related projects on https://jovian.ai/xdiad47/notebooks.


# FIFA-2020 to 2021 Players Data
In this notebook the analysis will be on FIFA players. Here we will find out the top players, top ten clubs, top ten richest clubs and many more. 
The dataset has been downloaded from Kaggle Dataset. The dataset contains a csv file i.e., players_20.csv. 
Libraries are used in this notbook are: Numpy, Pandas, Matplotlib and Seaborn. 
These libraries are covered in the course by Jovian.ml named as Data Analysis with Python: Zero to Pandas. 
As a first step, let's upload our Jupyter notebook to Jovian.ml.

### project_name = "FIFA-2020 to 2021 Players Data" 
### !pip install jovian --upgrade -q
### import jovian
### jovian.commit(project=project_name)

##Installing the upgraded version of all libraries
!pip install numpy pandas matplotlib seaborn --upgrade --quiet

## Importing the libraries
import numpy as np
import pandas as pd
import matplotlib
import matplotlib.pyplot as plt
import seaborn as sns
import warnings
warnings.filterwarnings("ignore")

## Global Settings
matplotlib.rcParams['font.size'] = 14
matplotlib.rcParams['figure.figsize'] = (15, 7.5)
matplotlib.rcParams['figure.facecolor'] = '#00000000'
sns.set_style("darkgrid")
## Reading players_20.csv into FIFA_21_df dataframe
FIFA_21_df = pd.read_csv('players_20.csv')
## showing FIFA_21_df
FIFA_21_df
