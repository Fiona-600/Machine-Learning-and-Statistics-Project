**Machine Learning and Statistics - 2021 Project Submission** <br/>
**GMIT Higher Diploma in Data Analytics** <br/>
**Submitted by Fiona Lee - 19 December 2021** <br/>

**Introduction**
***
This project provides an overview and demonstrations of the scikit-learn and scipy.stats packages. 

Repository Link: https://github.com/Fiona-600/Machine-Learning-and-Statistics-Project

![alt text](https://dataaspirant.com/wp-content/uploads/2014/10/scikit-learn-logo.png)

*Source: https://dataaspirant.com/wp-content/uploads/2014/10/scikit-learn-logo.png

<br/>

**Purpose of the project**
***

The elements explored will be:

1. An overview of the scikit-learn and scipy.stats packages 
2. Demonstrations of three scikit-learn algorithms
3. Demonstration of a hypothesis test using `ANOVA`, `T-test` and `Tukey` post hoc testing
4. Related visualisations and plots 

<br/>

***The Abalone Dataset***
***
<br/>

***About the Abalone Dataset***

Abalones are marine snails with an ear-shaped shell lined with mother of pearl. 56 species of abalones have been validated with an 18 additional subspecies.

The purpose of the analysis of the dataset is to predict the age of an abalone from its physical measurements (features) using machine learning rather than manually counting the number of rings on its shell.

![alt text](https://cdn.shopify.com/s/files/1/0206/7404/products/Abalone-Shell_grande.jpg?v=1500585184)

**Source Link:** https://cdn.shopify.com/s/files/1/0206/7404/products/Abalone-Shell_grande.jpg?v=1500585184 
<br/>

**Repository link to the dataset:** https://github.com/Fiona-600/Machine-Learning-and-Statistics-Project/blob/main/abalone.csv
<br/>
<br/>

***Features***

- 'Sex': M, F, and I (male, female, infant) 
- 'Length': Longest shell measurement (mm) 
- 'Diameter': Perpendicular to length (mm) 
- 'Height': Height with meat in shell (mm) 
- 'Whole weight': Whole abalone (grams) 
- 'Shucked weight': Weight of meat (grams) 
- 'Viscera weight': Gut weight after bleeding (grams) 
- 'Shell weight': Weight after being dried (grams) 

**Target**
- 'Age':  Number of Rings

<br/>

**Qualities and attributes of the Abalone dataset**

The original dataset contained 4176 samples (rows) and 9 variables (columns) namely: 'Sex','Length', 'Diameter', 'Height','Whole_Weight', 'Schucked_Weight', 'Viscera_Weight', 'Shell_Weight','Age'. 

The changes made to the original dataset were as follows:

- 2 samples with heights in excess of 0.5 mm were were deemed 'exceptional samples' and were removed from the dataset.  
- 5 samples with heights less than 0.02 mm were were deemed 'exceptional samples' and were removed from the dataset.  
<br/>
The Mean, Median, Standard Deviation, Min and Max Values for each variable are contained in the scikit.stats.ipynb file
<br/>
<br/>
<br/>

**The Wine Quality Dataset**
***
<br/>

***About the Wine Quality Dataset***

This dataset has the fundamental features which are responsible for affecting the quality of the wine. The purpose of the analysis of the dataset is to predict the quality of the wine from its features. 
<br/>

![alt text](https://3.bp.blogspot.com/-nNeSqByTMaE/TVT5RN0091I/AAAAAAAAAD4/B4iVB3dT4P0/s1600/New+Pictureqwe.jpg)
<br/>

**Source Link:** https://3.bp.blogspot.com/-nNeSqByTMaE/TVT5RN0091I/AAAAAAAAAD4/B4iVB3dT4P0/s1600/New+Pictureqwe.jpg

**Repository link to the dataset:** https://github.com/Fiona-600/Machine-Learning-and-Statistics-Project/blob/main/winequality-red.csv
<br/>

***Features***							

- 'Fixed acidity'
- 'volatile acidity'
- 'citric acid'
- 'residual sugar'
- 'chlorides'
- 'free sulfur dioxide'
- 'total sulfur dioxide'
- 'density'
- 'pH'
- 'sulphates'
- 'alcohol'

**Target**

- 'quality' 
<br/>
<br/>

**Qualities and attributes of the Wine Quality dataset**

The original dataset contained 1,599 samples (rows) and 12 variables (columns) namely: 'Fixed acidity', 'volatile acidity', 'citric acid', 'residual sugar', 'chlorides', 'free sulfur dioxide', 'total sulfur dioxide', 'density', 'pH', 'sulphates', 'alcohol', 'quality'.

The values in the 'quality' column were amended as follows:

- Result 1-4 replaced with 'Poor'
- Result 5-7 replaced with 'Good'
- Result 8-10 replaced with 'Excellent'
<br/>

The Mean, Median, Standard Deviation, Min and Max Values for each variable are contained in the scikit-learn.ipynb file

<br/>

**Research & Assumptions**
***
I made the assumption that samples in the abalone dataset with a height less than 0.02mm and greater than 0.5mm were incorrectly collated so they were excluded.

<br/>

**Conclusions and Findings**
***
<br/>

**Structure & Project Navigation**
***

The project will be stored in a GITHUB repository at url: https://github.com/Fiona-600/Machine-Learning-and-Statistics-Project
<br/>

The GITHUB repository contains:

• A *‘gitignore’* file containing any files or file types which should be ignored by the github repository

• A *‘LICENSE’* file containing a copy of the MIT Licence

• A *'project-instructions.pdf'* file which outlines detailed instructions for the project 

• A *‘README.md’* file which contains:

  1.	The purpose of the project 
  2.  Information about the datasets
  3.	Research and assumptions 
  4.	Conclusions and findings  
  5.	Structure and project navigation
  6.	Required programs
  7.	Details of how to run the code 
  8.	Libraries and modules which need to be imported to run the code
  9.	Authors and contributors
  10.	References

• A *‘requirements.txt’* file containing information that facilitates the user to quickly run the notebooks with minimal configuration

• A python program file called *‘scikit-learn.ipynb’* which contains the following:

  1. A demonstration of the following three scikit-learn algorithms:

    •	
    •	
    •	
  
  2.	Related visualisations and plots for each algorithm
<br/>

• A python program file called *‘scikit-stats.ipynb’* which contains:

  1.	A demonstration of a hypothesis test using ANOVA
  
  2.	Related visualisations and plots

<br/>

**Required Programs**
***
- Anaconda Navigator 3 - https://www.anaconda.com/
- Jupyter Notebook - https://jupyter.org/install  
- Python version 3.8.8 - downloaded via Anaconda Navigator 3 to Windows 10 operating system
- Cmder Console Emulator - https://cmder.net/
- GitHub Repository Storage - https://github.com/
- Firefox Internet Explorer - https://www.mozilla.org/en-US/firefox/new/

<br/>

**Opening and running the code in the Jupyter Notebook**
***
  1.	Navigate to your desired location on your local drive using CMDER
  2.  If you do not already have an SSH key, you will need to generate a new SSH key to use for authentication by typing the following into CMDER: ssh-keygen -t ecdsa-sk -C "your_email@example.com" (replace your e-mail address) and then save and choose a security passphrase.
  2.  Clone the github repository onto your local drive by using the command 'git clone git@github.com:Fiona-600/Machine-Learning-and-Statistics-Project.git' in CMDER.
  4.  Use the command 'Jupyter notebook' in CMDER to open Jupyter Notebook in your browser and navigate to the chosen file to view.  Note do not close this window as his will end the connection with your browser.
  4.	Use 'Restart and Run All' in the 'Kernel' tab in Jupyter Notebook to refresh and re-run the entire code
  5.	Hold 'Shift' + 'Enter' to run/test code in individual code cells in a Jupyter Notebook

<br/>

**Libraries and Modules**
***
*scikit-learn.ipynb file:*

- Pandas - 'import pandas as pd'
- Numpy - 'import numpy as np'
- Matplotlib - 'import matplotlib.pyplot as plt'
- Seaborn- 'import seaborn as sns'
- Model selection - 'import sklearn.model_selection as mod' 
- Linear regression - 'import sklearn.linear_model as lm'
- K nearest neighbours - 'import sklearn.neighbors as nei'
- LogisticRegression - 'from sklearn.linear_model import LogisticRegression as log'
- Confusion matrix - 'from sklearn.metrics import accuracy_score, precision_score, confusion_matrix as score'
- Train, Test, Split - 'from sklearn.model_selection import train_test_split'
- Classification Report - 'from sklearn.metrics import classification_report'
- Decision Tree Classifier - 'from sklearn.tree import DecisionTreeClassifier'

*scipy.stats.ipynb file:*

- Pandas dataframes - 'import pandas as pd'
- Seaborn- 'import seaborn as sns'
- Matplotlib - 'import matplotlib.pyplot as plt'
- Scipy.stats - 'import scipy.stats as ss'
- Numpy - 'import numpy as np'
- Collections - 'import collections as co'
- Specials - 'import scipy.special as spec'
- Anova - import scipy.stats as stats
- Norm - 'from scipy.stats import norm'
- Anova one way - 'from scipy.stats import f_oneway'
- Tukey HSD- 'from statsmodels.stats.multicomp import pairwise_tukeyhsd'

<br/>

**Author & Contributors**
***
**Author:** Fiona Lee

**Contributors:** I relied heavily on the tutorials in Ian McLoughlin's Github repository at https://github.com/ianmcloughlin/jupyter-teaching-notebooks

With thanks to Ian for all the helpful tips in completing this project.

<br/>

**References**
***
[1] <br/>
[2] <br/>
[3] <br/>
[4] <br/>
[5] <br/>
[6] <br/>
[7] <br/>
[8] <br/>
[9] <br/>
[10] <br/>