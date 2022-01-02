**Machine Learning and Statistics - 2021 Project Submission** <br/>
**GMIT Higher Diploma in Data Analytics** <br/>
**Submitted by Fiona Lee - 2 January 2022** <br/>

**Introduction**
***
This project provides an overview and demonstration the uses of the scikit-learn and scipy-stats packages. 

Repository Link: https://github.com/Fiona-600/Machine-Learning-and-Statistics-Project

![alt text](https://dataaspirant.com/wp-content/uploads/2014/10/scikit-learn-logo.png)

*Source: https://dataaspirant.com/wp-content/uploads/2014/10/scikit-learn-logo.png

<br/>

**Purpose of the project**
***

The elements explored will be:

1. An overview of the scikit-learn and scipy-stats packages 
2. Demonstrations of three scikit-learn algorithms i.e. Decision Tree Classifier, Random Forests Classifier and Linear Regression Algorithms
3. Demonstration of a hypothesis test using `ANOVA`, `T-test`, `Shapiro Wilk test`, `Levine test` and `Tukey` post hoc testing
4. Related visualisations and plots 

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

**Qualities and attributes of the Wine Quality dataset**

The original dataset contained 1,599 samples (rows) and 12 variables (columns) namely: 'Fixed acidity', 'volatile acidity', 'citric acid', 'residual sugar', 'chlorides', 'free sulfur dioxide', 'total sulfur dioxide', 'density', 'pH', 'sulphates', 'alcohol', 'quality'.

The values in the 'quality' column were amended as follows:

- Result 1-4 replaced with 'Poor'
- Result 5-7 replaced with 'Good'
- Result 8-10 replaced with 'Excellent'
<br/>

The Mean, Median, Standard Deviation, Min and Max Values for each variable are contained in the scikit-learn.ipynb file

<br/>
<br/>
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

- 2 samples with heights in excess of 0.3mm were were deemed 'exceptional samples' and were removed from the dataset.  
- 5 samples with heights less than 0.02mm were were deemed 'exceptional samples' and were removed from the dataset.  
<br/>
The Mean, Median, Standard Deviation, Min and Max Values for each variable are contained in the scipy.stats.ipynb file
<br/>
<br/>
<br/>

**Research & Assumptions**
***
I made the assumption that samples in the abalone dataset with a height less than 0.02mm and greater than 0.5mm were incorrectly collated so they were excluded.
<br/>
No changes were made to the wine quality dataset other than classifying quality as excellent, good or poor based on the score from 1-10 in the dataset.
<br/>
<br/>
**Conclusions and Findings**
***
It was concluded that the wine quality dataset was highly suited to classification algorithms such as the decision tree classifier and random forest classifier.  The algorithms applied predicted within a 5% and 9% margin of error the quality of a wine depending on it's features. 

The abalone dataset was less successful in predicting the age of the specimen based on its' physical attributes.  The algortithm successfully predicted the correct outcome in 52% of test cases.  This was likely due to the fact that there was a wide range of values between adult and infant specimens.
<br/>
<br/>

**Structure & Project Navigation**
***

The project will be stored in a GITHUB repository at url: https://github.com/Fiona-600/Machine-Learning-and-Statistics-Project
<br/>

The GITHUB repository contains:

• A *‘gitignore’* file containing any files or file types which should be ignored by the github repository

• *'abalone.csv'* file containing the abalone dataset

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

    •	Decision Tree Classifier applied to the 'Wine Quality Dataset'
    •	Random Forests Classifier applied to the 'Wine Quality Dataset'
    •	Linear Regession Algorithm applied to the 'Abalone Dataset'
  
  2.	Related visualisations and plots for each algorithm
<br/>

• A python program file called *‘scipy-stats.ipynb’* which contains:

  1.	A demonstration of a hypothesis test using `ANOVA`, `T-test`, `Shapiro Wilk test`, `Levine test` and `Tukey` post hoc testing
  
  2.	Related visualisations and plots

• *'winequality-red.csv'* file containing the wine quality dataset

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

**Installing the requirements.txt file**
- Use 'pip install -r requirements.txt' in the  to install the file of Python packages.

<br/>

**Opening and running the code in the Jupyter Notebook**
***
  1.	Navigate to your desired location on your local drive using CMDER
  2.  If you do not already have an SSH key, you will need to generate a new SSH key to use for authentication by typing the following into CMDER: ssh-keygen -t ecdsa-sk -C "your_email@example.com" (replace your e-mail address) and then save and choose a security passphrase.
  2.  Clone the github repository onto your local drive by using the command 'git clone git@github.com:Fiona-600/Machine-Learning-and-Statistics-Project.git' in CMDER.
  4.  Whilst still in the location of the file on your local drive, use the command 'Jupyter notebook' in CMDER to open Jupyter Notebook in your browser and navigate to the chosen file to view.  Note do not close this window as his will end the connection with your browser.
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
- Accuracy Score, Precision Score & Confusion Matrix - 'from sklearn.metrics import accuracy_score, precision_score, confusion_matrix as score'
- Model selection - 'import sklearn.model_selection as mod' 
- Linear regression - 'import sklearn.linear_model as lm'
- Model selection - 'from sklearn.model_selection import train_test_split'
- LogisticRegression - 'from sklearn.linear_model import LogisticRegression as log'
- Classification Report - 'from sklearn.metrics import classification_report'
- Decision Tree Classifier - 'from sklearn.tree import DecisionTreeClassifier'
- Random Forests Classifier - from sklearn.ensemble import RandomForestClassifier


*scipy-stats.ipynb file:*

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

**Contributors:** I used the tutorials in Ian McLoughlin's Github repository at https://github.com/ianmcloughlin/jupyter-teaching-notebooks for reference

With thanks to Ian for all the helpful tips in completing this project.

<br/>

**References**
***
*scikit-learn.ipynb file:*
<br>

[1] https://www.tutorialspoint.com/scikit_learn/scikit_learn_introduction.html

[2] https://www.tutorialspoint.com/scikit_learn/scikit_learn_tutorial.pdf

[3] https://www.springboard.com/library/machine-learning-engineering/scikit-learn-vs-tensorflow/#:~:text=Scikit-Learn%20is%20an%20open-source%20package%20for%20creating%20and,includes%20tools%20to%20help%20you%20preprocess%20your%20dataset.

[4] https://machinelearningmastery.com/supervised-and-unsupervised-machine-learning-algorithms/

[5] https://dataaspirant.com/unsupervised-learning-algorithms/

[6] https://www.tutorialspoint.com/scikit_learn/scikit_learn_modelling_process.html

[7] https://www.geeksforgeeks.org/introduction-to-factor-analytics/#:~:text=The%20factor%20analysis%20technique%20extracts%20the%20maximum%20common,so%20it%20is%20quite%20related%20to%20data%20mining. 

[8] https://www.simplilearn.com/10-algorithms-machine-learning-engineers-need-to-know-article#:~:text=%20List%20of%20Popular%20Machine%20Learning%20Algorithms%20,learning%20is%20one%20of%20the%20most...%20More%20

[9] https://archive.ics.uci.edu/ml/datasets/Abalone

[10]https://www.researchgate.net/profile/Ayodejilearning:Salau/publication/330702663/figure/fig2/AS:720339474587651@1548753722728/Machine-learning-algorithms-a-Supervised-learning-In-this-type-of-learning-the-output.ppm

[11] https://www.kaggle.com/rodolfomendes/abalone-exploratory-data-analysis

[12] scikit-learn.org/stable/index.html

[13] https://stackabuse.com/decision-trees-in-python-with-scikit-learn/ 

[14] https://medium.com/analytics-vidhya/visually-interpreting-the-confusion-matrix-787a70b65678 

[15] https://github.com/ianmcloughlin/jupyter-teaching-notebooks

*scipy-stats.ipynb file:*
<br/>
[1] https://docs.scipy.org/doc/scipy/reference/stats.html

[2] https://www.tutorialspoint.com/scipy/scipy_stats.htm

[3] http://specminor.org/2017/01/11/python-descriptive-statistics-scipy.html#:~:text=The%20statistics%20library%20par%20excellence%20for%20Python%20is,bunch%20of%20descriptive%20statistics%20at%20once%2C%20scipy.stats.describe%20%28%29%3A

[4] https://programming-review.com/python/scipy-examples#:~:text=Statsmodels%20has%20scipy.stats%20as%20a%20dependency.%20Scipy.stats%20has,it%20works%20with%20pandas%20out%20of%20the%20box

[5] https://docs.scipy.org/doc/scipy/reference/stats.html

[6] https://data-flair.training/blogs/scipy-statistical-functions/#:~:text=The%20scipy.stats%20is%20the%20SciPy%20sub-package.%20It%20is,functionality%20is%20expanding%20as%20the%20library%20is%20open-source.

[7] https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.rv_continuous.html

[8] https://www.bing.com/search?q=cdf+method&cvid=c65ee34bfef34d37ba0399662d25bbbe&aqs=edge.0.0j69i57j0l3.2763j0j1&pglt=163&FORM=ANNTA1&PC=U531

[9] https://support.minitab.com/en-us/minitab-express/1/help-and-how-to/basic-statistics/probability-distributions/how-to/cumulative-distribution-function-cdf/methods-and-formulas/methods-and-formulas/#:~:text=%20Methods%20and%20formulas%20for%20Cumulative%20Distribution%20Function,a%20standard%20normal%20distribution%2C%20X%202...%20More%20

[10] https://integratedmlai.com/normal-distribution-an-introductory-guide-to-pdf-and-cdf/#:~:text=The%20probability%20density%20function%20%28PDF%29%20is%20a%20statistical,the%20interval%20in%20which%20the%20variable%20will%20fall.

[11] https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.shapiro.html

[12] https://statistics.laerd.com/spss-tutorials/testing-for-normality-using-spss-statistics.php

[13] https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.shapiro.html

[14] https://www.spss-tutorials.com/spss-shapiro-wilk-test-for-normality/

[15] https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.levene.html

[16] https://statistics.laerd.com/statistical-guides/independent-t-test-statistical-guide.php

[17] https://seaborn.pydata.org/generated/seaborn.boxplot.html

[18] https://splendidwritings.com/testing-assumptions-the-shapiro-wilk-test-and-the-levene-test/

[19] https://www.geeksforgeeks.org/how-to-plot-normal-distribution-over-histogram-in-python/

[20] https://statistics.laerd.com/spss-tutorials/one-way-anova-using-spss-statistics.php

[21] https://www.scribbr.com/statistics/one-way-anova/

[22] https://nathancarter.github.io/how2data/site/how-to-perform-post-hoc-analysis-with-tukey-s-hsd-test-in-python-using-statsmodels-matplotlib-and-scikit/

[23] https://www.statology.org/tukey-test-python/

[24] https://towardsdatascience.com/anova-test-with-python-cfbf4013328b

[26] https://github.com/ianmcloughlin/jupyter-teaching-notebooks

