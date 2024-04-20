# Regression model project for marketing

## Introduction:

A company is investing monthly in online advertising platforms, such as YouTube, Facebook, and newspapers, to prospect for leads. To track the performance of these investments, the company records all advertising expenditures and sales returns generated. The company approached us to better understand the relationship between these variables and identify factors that most impact lead generation. Furthermore, the company seeks to create a model to predict sales returns from advertising investments. This project used the CRISP-DM model.

### Project's goal:
- Analyze the collected data.
- Visualize data to identify relationships and patterns.
- Create a model to predict sales returns.

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

- This analysis using the bar graph helped visualize how investments are distributed among different media categories and compare their impact on total sales. It led to the conclusion that investing in YouTube media has a greater impact on the result.
<p align="center">
<img  width="80%" src="https://github.com/Joaovtmendes/Marketing-regression/assets/154254190/561c0797-d05a-4b48-8589-51ee9aef0f77">
</p>

- This scatter plot shows the relationship between advertising spend on different media (YouTube, Facebook, and Newspaper) and the resulting sales. Each point represents a unique observation, with its position indicating the amounts spent on each medium and the resulting sales.

  - Analyzing the data, we observe a positive correlation between advertising spend on YouTube and sales, suggesting that increasing investment in YouTube advertising leads to higher sales. This indicates that YouTube advertising is effective in driving sales.

  - For Facebook, we also observe a positive correlation, but with the presence of significant outliers. These outliers had a negative impact on sales, representing exceptional advertising strategies that deviated from the general trend and resulted in lower sales. These outliers highlight the importance of carefully evaluating advertising strategies to avoid negative outcomes.

  - In contrast, spending on Newspaper advertising shows uncorrelated data, indicating no clear relationship between spending on Newspaper advertising and sales. This suggests that Newspaper advertising may not have a significant impact on sales, or that other factors not captured in the data are influencing the results.
<p align="center">
<img  width="80%" src="https://github.com/Joaovtmendes/Marketing-regression/assets/154254190/eadbf2fd-bbdb-467d-a821-85090ad4ef45">
</p>

- To further reinforce the correlation observed in the scatter plot above, a heatmap graph was used to calculate the correlation matrix between all numerical variables in the DataFrame. Each value in the matrix represents the correlation between two variables, ranging from -1 to 1. A value closer to 1 indicates a strong positive correlation, while a value closer to -1 indicates a strong negative correlation. A value close to 0 indicates a lack of correlation. This analysis was important to emphasize that the relationship between the amount invested in YouTube directly impacts the value of sales.
<p align="center">
<img  width="60%" src="https://github.com/Joaovtmendes/Marketing-regression/assets/154254190/e721aeca-4eb9-4ab8-a68b-8d920e611777">
</p>

- The histogram was used to visualize how different levels of investment are related to sales returns, providing insights into the effectiveness of advertising strategies in each medium. In this case, it can be seen that the majority of advertising investments resulted in an average return on sales. This suggests that, despite the investments, the return was not exceptionally high or low in most cases. The analysis indicates the need to evaluate and adjust advertising strategies to seek a more significant return on the investments made.
<p align="center">
<img  width="60%" src="https://github.com/Joaovtmendes/Marketing-regression/assets/154254190/82a9d761-a58b-4e59-805b-fe4b4e162616">
</p>
  
## Solution:

- We have developed a regression model that helps the client test different investment strategies and visualize the return on investment (ROI). By identifying the optimal distribution of spending across each media channel, we can predict the potential return and align with the advertising team on the best strategy.

  - In the tabs of the platforms below, values can be entered to carry out a sales simulation according to the investment:

youtube = x </p>
facebook = y </p>
newspaper = z </p>

investment = [[youtube,facebook,newspaper]]</p>
forecast_sales = regXGB.predict(investment)</p>
print('Sales forecast:', forecast_sales[0])




















