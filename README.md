# House_Prices-Advanced-Regression-Techniques

This is a public competition on Kaggle:  [House Prices: Advanced Regression Techniques](https://www.kaggle.com/c/house-prices-advanced-regression-techniques)

Trying to predict sales prices of houses.  Dataset has 81 features.
The Challenge was to find out which features might be predictive of sale price.

While performing my own train/test split, my model was able to achieve a score of up to 86-88% (10 feature model and 44 feature model).

For the competition with the actual test dataset, my submission received the best score of .15% (Root Mean Squared Logarithmic Error).  This was good enough to place in the top 3,000.  The model that received the best score, was my model which only used 10 features to train and predict on.

I performed this work by myself, without the aid of a team.

Please check my [Jupyter Notebook](House_Prices-Advanced-Regression-Techniques/EDA.ipynb)

For some data visualization, please see the below:
* I used a [correlation heat map](CorrelationHeatMap1.png), to see which features may be [highly correlated](CorrelationHeatMap2.png) to possibly eliminate features.
* [The original distribution of sales price](SalePriceDistribution.png)
* [After I transformed the sale price with the natural log, so it would be normally distributed](After-LogSalePriceDistribution.png)
* [Showing the relationship between price and Neighborhood](SalePrice_v_Neighborhood.png).  I ended up combining some neighborhoods that showed similar pricing, and then dummied them, because this was 25, and I combined them down to 4.
* One category I created, was [TotalSF](SalePrice_v_TotalSF.png).  This was a combination of 1stFloor, 2ndFloor, Basement Square Footage, and I believe this ended up showing a more linear positive relationship, than any of the others did by themselves, when compared to the SalesPrice.
