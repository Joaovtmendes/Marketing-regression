# Regression model project for marketing

## Introduction:

A company is investing monthly in online advertising platforms, such as YouTube, Facebook and newspapers, to prospect for leads. In order to track the performance of these investments, the company records all advertising expenditures and all sales returns generated from these investments. The company approached us with the aim of better understanding the relationship between the variables present in these records and identifying the factors that most impact lead generation. Furthermore, the company seeks to create a value prediction model to estimate the sales return that can be generated from a given investment in advertising.
To carry out this project, the CRISP-DM model was used.

### Project's goal:
- Analyze the collected data.
- Graphical display of data to identify relationships between variables and discover relevant patterns.
- Create a value prediction model to estimate sales return.

### Technologies Used:
<p align="left">  
  <a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> 
  <a href="https://pandas.pydata.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/2ae2a900d2f041da66e950e4d48052658d850630/icons/pandas/pandas-original.svg" alt="pandas" width="40" height="40"/> </a> 
  <a href="https://numpy.org/" target="_blank" rel="noreferrer"> <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/numpy/numpy-original.svg" alt="numpy" width="40" height="40"/> 
  <a href="https://matplotlib.org/" target="_blank" rel="noreferrer"> <img src="https://seeklogo.com/images/M/matplotlib-logo-7676870AC0-seeklogo.com.png" alt="matplotlib" width="40" height="40"/> 
  <a href="https://scikit-learn.org/" target="_blank" rel="noreferrer"> <img src="https://upload.wikimedia.org/wikipedia/commons/0/05/Scikit_learn_logo_small.svg" alt="scikit_learn" width="40" height="40"/> </a>
  <a href="https://seaborn.pydata.org/" target="_blank" rel="noreferrer"> <img src="https://seaborn.pydata.org/_images/logo-mark-lightbg.svg" alt="seaborn" width="40" height="40"/> </a> 

## Data collection:

At this stage, a csv file was imported containing the amounts invested monthly on the platforms: Youtube, Facebook and newspaper, and the return on sales of this investment.

## Data Preparation:

To prepare the data, the Pandas libraries were used to perform the following functions:
Pandas: https://pandas.pydata.org/docs/user_guide/index.html#user-guidefunções:
- Evaluated if there were null numbers:
- Evaluated whether there were duplicate lines
- Evaluated the discretion and count of each column

## Modeling techniques:

For the exploratory analysis stage, the Seaborn and Plotly libraries were used to identify relationships between variables and discover relevant patterns.
- Seaborn: https://seaborn.pydata.org/tutorial.html
- Plotly: https://plotly.com/python-api-reference/

For the model training stage, the scikit-learn library was used.
- Scikit-learn: https://scikit-learn.org/stable/model_selection.html

For the modeling stage, the XGboost library was used to make a decision tree model. A comparison was made between the regression models with sklearn and XGBoost and the MSE and RMSE values were lower in XGBoost, which is why this model was used.
- XGboost regression https://xgboost.readthedocs.io/en/stable/python/python_api.html

## Results:


























