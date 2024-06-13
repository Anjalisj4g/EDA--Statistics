# EDA--Statistics

The project aims at examining the price per square feet coloumn of a dataset "House price", checking for outliers, removing outliers, plotting histogram and scatter plot and finding skewness and kurtosis before and after transformation.

I have done some basic EDA using functions info, describe, head, tail, columns etc.
There were 13200 rows and 7 columns.

I have plotted a pairplot to get a baisc understanding of relationship between various numerical and categorcal columns.

# Data Preprocessing

I plotted a distplot to check whether there was any outliers. There were many outliers.

For removing outliers, I have used for methods :
* By using mean and standard deviation
* Z-score method
* Percentile method
* Interquartile method.

I have used both trimming and capping method to remove outliers. Capping is better because it won't remove any row.

# Interquartile method worked best out of all the methods. It removed almost all the outliers.#

I have drawn a histplot with the given data. It was not normally distributed. 
* Skewness = 108, which means highly right skewed
* Kurtosis = 12093, which means graph is leptokurtic.

Then, I applied logarithmic transformation on it. The distplot after transformation was almost normally distributed.
* Skewness = 1.3, which is nearer to 1. So, the graph is less skewed.
* Kurtosis = 12, which is very less compared with before transformation. It is leptokurtic since kurtosis is greater than 3.

Checked correlation between numerical columns and drawn heatmaps.

There is a very less linear relationship among column price_per_sqft and bath, price and bhk.
There is an inverse relationship between column price_per_sqft and total_sqft.
There is a good linear relationship between bath and bhk.

Represented the relationship between various columns using scatter plot.

  
