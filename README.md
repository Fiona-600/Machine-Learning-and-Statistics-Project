**Fundamentals of Data Analysis 2020 Project Submission**

**GMIT Higher Diploma in Data Analytics**

**Submitted by Fiona Lee - 8 January 2021**

**Introduction**

This project uses 'Simple Linear Regression' to predict the power output of wind turbines based on a given wind speed using the 'Wind-Power' dataset as the basis.

![alt text](https://www.munichre.com/content/dam/assets/munichre/images/royalty-free-ppt-only/200416688-001_22.jpg/_jcr_content/renditions/original.image_file.5079.2857.0,329,5079,3186.file/200416688-001_22.jpg)

*Source: https://www.munichre.com/content/dam/assets/munichre/images/royalty-free-ppt-only/200416688-001_22.jpg/_jcr_content/renditions/original.image_file.5079.2857.0,329,5079,3186.file/200416688-001_22.jpg*

**Qualities and attributes of the Wind-Power dataset**

The original dataset contained 500 samples (rows) and 2 variables (columns) namely: 'speed' and 'power'. 

The changes made to the original dataset are as follows:

- The 'speed' and 'power' headers were renamed as 'Speed_Mph' and 'Power_KWph'
- 15 samples were deemed either 'test' or 'exceptional samples' and were removed from the dataset.  
- Additional columns were added i.e 'Power:Speed','Classification','Cost' and 'Power_Prediction'  

**The Mean, Median, Standard Deviation, Min and Max Values for each variable are contained in the Final Project 2020.ipynb file**

*Repository Link: https://github.com/Fiona-600/Fundamentals-of-Data-Analytics-2020-Project/blob/main/Final%20Project%202020.ipynb*

**Purpose of the project**

The elements explored will be:

1.	'Simple Linear Regression' as applied to the 'Wind-Power' data set 
2.	Explanation of the simple linear regression method and an analysis of its' accuracy
3.	Prediction of power output based on a given wind speed
4.	Use of other types of regression methods to produce the same output as the simple linear regression approach


**Research & Assumptions**

Wind turbines typically start operating at wind speeds around 8-12 miles per hour (mph). Turbines reach maximum power output at 25-30 mph. At very high wind speeds, i.e. 55 mph or greater the wind turbines shut down to prevent excessive wear and tear. 

(source: https://enerpower.ie/portfolio/wind-turbine-faq-ireland/)

Power:speed ratio is recommended to be between 6 and 8 eg. for a grid connected wind turbine with 3 blades, the optimum ratio is suggested as 7. 

(source: https://www.mdpi.com/)

Based on the research above, I decided on the following assumptions:

1.	Low or no power output at wind speeds below 8 mph is normal 
2.	Zero wind speed and power output is most likely test data 
3.	A power:speed ratio between 6 and 8 is optimal
4.	A power:speed ratio less than 6 is sub-optimal
5.	A power:speed ratio greater than 8 is exceptional


**Simple Linear Regression**

Simple linear regression is an approach for predicting a response using a single feature.  It is assumed that there are two linearly related variables, a feature (Speed_Mph) and a response (Power_KWph). 

This method attempts to find a linear function that predicts the response value (in this case Power_KWph) as accurately as possible as a function of the feature variable (Speed_Mph).

The line which best fits the plot of the dataset is called 'regression line'.  This line is used to predict a feature value i.e.  'Power_KWph' which is not already present in dataset.

The equation of regression line is represented as:

y = (intercept + slope (x))

source: https://www.geeksforgeeks.org/linear-regression-python-implementation/

**Conclusions and Findings**

The data in the Wind-Power datasets suggest that the 90% (439) of the samples selected have performed below the power:speed ratio standard for wind turbines of 6. There is exponential growth in power output between wind speeds of 8 and 18 mph and relatively flat output between 0 to 8mph and 18 to 25 mph.

The Wind-Power dataset is not a perfect linear example for simple linear regression.  The dataset follows a curved shape with two bends (cubic) when plotted so it is difficult to fit a line closely to the data.  

The cost of the best fit line of 80,618 represents the sum of the individual differences between predicted and actual values for y (i.e. Power_KWph) squared.  This reflects the poor fit of the line.

In contrast, the 'R-squared' value result is 90% which suggests that 90% of the values fall within the regression line region.  On inspection of the graph vs 'best line' plot however this does not appear to be the case.  This is because the regression line consistently under and over-predicts the data along the curve, which is bias. The ideal scenario for using simple linear regression is an unbiased model with residuals that are randomly scattered around zero.


**Structure & Project Navigation**

The project will be stored in a GITHUB Repository at url: https://github.com/Fiona-600/Fundamentals-of-Data-Analytics-2020-Project

The GITHUB repository contains:

    •	A ‘gitignore’ file containing any files or file types which should be ignored by the github repository  
    
    •	A python program file called ‘Final Project 2020.ipynb’ which contains:
 
          •	Online and other research into simpple linear regression and other approaches
          •	High level review and summary of the data set
          •	Identification of trends and exceptional samples (outliers)      
          •	Visualisation of the data set and the relationship between the variables
          •	Prediction models using simple linear regression and sklearn approaches
    
    •	A ‘LICENSE’ file containing a copy of the MIT Licence

    •	A ‘README.md’ file which contains:

          •	Introduction to the dataset 
          •	Explanation of the 'simple linear regression' 
          •	Conclusions and findings        
          •	How to run the python code
          •	References used in completing the project

    •	Wind-Power.csv - Wind Speed/Power Dataset


**Required Programs**

	•	Anaconda Navigator 3 - https://www.anaconda.com/
	•	Jupyter Notebook - https://jupyter.org/install  
	•	Python version 3.8.3 - downloaded via Anaconda Navigator 3 to Windows 10 OS
	•	Cmder Console Emulator - https://cmder.net/
 	•	GitHub Repository Storage - https://github.com/
	•	Firefox Internet Explorer - https://www.mozilla.org/en-US/firefox/new/


**Opening and running the code in the Jupyter Notebook**

    •	NumPy - ‘import numpy as np’
    •	Pandas – ‘import pandas as pd’ 
	•	Clone or download the 'FinalProject.ipynb' file from Github onto your local drive
	•	Open the Jupyter Notebook file in your browser using CMDER
	•	Use 'Restart and Run All' in the 'Kernel' tab in Jupyter Notebook to re-run the entire code
	•	Hold 'Shift' + 'Enter' to run/test code in individual code cells in a Jupyter Notebook


**Libraries and Modules**

    •	NumPy - ‘import numpy as np’
    •	Pandas – ‘import pandas as pd’   
    •	From Pandas import Dataframe’       
    •	Matplotlib - ‘import matplotlib.pyplot as plt’
    •	from sklearn.metrics import r2_score 
    •	from sklearn import linear_model  
    •	from sklearn.linear_model import LinearRegression  


**Author & Contributors**

Fiona Lee


**License**

This project is licensed under the MIT License - see the LICENSE.md file for details


**Acknowledgments**

Ian McLoughlin for all the helpful tips in completing this assignment


**References**

https://realpython.com/linear-regression-in-python/

https://towardsdatascience.com/linear-regression-detailed-view-ea73175f6e86

https://machinelearningmastery.com/a-gentle-introduction-to-scikit-learn-a-python-machine-learning-library/

https://datatofish.com/sort-pandas-dataframe/

https://www.kite.com/python/answers/how-to-print-an-entire-pandas-dataframe-in-python

https://www.codegrepper.com/code-examples/python/how+to+align+column+name+to+center+in+pandas+dataframe

https://www.dataquest.io/blog/settingwithcopywarning/

https://realpython.com/pandas-groupby/

https://github.com/ianmcloughlin/jupyter-teaching-notebooks/blob/master/simple-linear-regression.ipynb

https://www.geeksforgeeks.org/python-coefficient-of-determination-r2-score/

https://medium.com/towards-artificial-intelligence/calculating-simple-linear-regression-and-linear-best-fit-an-in-depth-tutorial-with-math-and-python-804a0cb23660#9a2b

https://colab.research.google.com/drive/1WRdDbFFykiLv16-Vv-ghsregmfdbwtRX?usp=sharing&pli=1#scrollTo=3kbMmi6JYeB4

https://www.shanelynn.ie/select-pandas-dataframe-rows-and-columns-using-iloc-loc-and-ix/

https://datatofish.com/random-rows-pandas-dataframe/

https://scikit-learn.org/stable/auto_examples/linear_model/plot_ols.html

https://contactsunny.medium.com/linear-regression-in-python-using-scikit-learn-f0f7b125a204

https://stackabuse.com/linear-regression-in-python-with-scikit-learn/

https://www.geeksforgeeks.org/linear-regression-python-implementation/

https://enerpower.ie/portfolio/wind-turbine-faq-ireland/

https://www.mdpi.com/

