# Machine_Learning_PclubRoadmap
Machine_Learning_PclubRoadmap

## Object Oriented Programming( OOPS )

+ Every thing we define in python is a an object of a specific class as seen in example 1 output.
+ There are methods for which each object which are defined.
+ When u define a class of ur own and see the type it is __main__.classname. Here main is called the module and by default it is set to main. 
+ Init is a method which is automatically called whenever we define a object of a class. 
+ Self is an attribute which is defined to point to a specific object of the class for which it is called. 
+ When we inherit a class into another class, the class can use the methods of the inherited class.
+ We can inherit multiple classes into a single class. 

## KNN

+ kNN classifier identifies the class of a data point using the majority voting principle. If k is set to 5, the classes of 5 nearest points are examined. Prediction is done according to the predominant class. Similarly, kNN regression takes the mean value of 5 nearest locations.
+ There are various techniques to estimate the distance. Euclidean distance (Minkowski distance with p=2) is one of the most regularly used distance measurements. The graphic below explains how to compute the euclidean distance between two points in a 2-dimensional space. It is determined using the square of the difference between x and y coordinates of the locations.
+ Finally, considering all we’ve discussed so far, we should keep in mind that KNN isn’t ideal for large-dimensional datasets.

Conclusion
Hopefully, you now have a better understanding of the KNN algorithm. We’ve looked at a variety of ideas for how KNN saves the complete dataset in order to generate predictions.

KNN is one of several lazy learning algorithms that don’t use a learning model to make predictions. By averaging the similarity between an incoming observation and the data already available, KNN creates predictions on the fly (just in time).

## EDA 

What is EDA ?

Exploratory data analysis (EDA) is used by data scientists to analyze and investigate data sets and summarize their main characteristics, often employing data visualization methods.

EDA helps determine how best to manipulate data sources to get the answers you need, making it easier for data scientists to discover patterns, spot anomalies, test a hypothesis, or check assumptions

The main purpose of EDA is to help look at data before making any assumptions. It can help identify obvious errors, as well as better understand patterns within the data, detect outliers or anomalous events, find interesting relations among the variables.

### EDA TOOLS

Specific statistical functions and techniques you can perform with EDA tools include:

+ Clustering and dimension reduction techniques, which help create graphical displays of high-dimensional data containing many variables
+ Uni variate visualization of each field in the raw dataset, with summary statistics. 
+ Bivariate visualization and summary statistics that allow you to assess the relationship between each variable in the dataset and the target variable you're looking at. 
+ Multivariate visualizations for mapping and understanding interactions between different fields in the data.
+ K-means clustering, which is a clustering method in unsupervised learning where data points are assigned into K groups, i.e. the number of clusters, based on the distance from each group’s centroid. The data points closest to a particular centroid will be clustered under the same category. K-means clustering is commonly used in market segmentation, pattern recognition, and image compression.
+ Predictive models, such as linear regression, use statistics and data to predict outcomes. 

### Types of EDA
There are four primary types of EDA : 
+ Univariate non-graphical
+ Univariate graphical 
+ Multivariate non-graphical
+ Multivariate graphical

Univariate non-graphical : 
This is simplest form of data analysis, where the data being analyzed consists of just one variable. Since it’s a single variable, it doesn’t deal with causes or relationships. The main purpose of univariate analysis is to describe the data and find patterns that exist within it.

Univariate graphical : 
Non-graphical methods don’t provide a full picture of the data. Graphical methods are therefore required. Common types of univariate graphics include:

Stem-and-leaf plots, which show all data values and the shape of the distribution.

Histograms, a bar plot in which each bar represents the frequency (count) or proportion (count/total count) of cases for a range of values.

Box plots, which graphically depict the five-number summary of minimum, first quartile, median, third quartile, and maximum.

Multivariate nongraphical : 
Multivariate data arises from more than one variable. Multivariate non-graphical EDA techniques generally show the relationship between two or more variables of the data through cross-tabulation or statistics

Multivariate graphical : 
Multivariate data uses graphics to display relationships between two or more sets of data. The most used graphic is a grouped bar plot or bar chart with each group representing one level of one of the variables and each bar within a group representing the levels of the other variable.

Other common types of multivariate graphics include:

Scatter plot, which is used to plot data points on a horizontal and a vertical axis to show how much one variable is affected by another.

Multivariate chart, which is a graphical representation of the relationships between factors and a response.

Run chart, which is a line graph of data plotted over time.

Bubble chart, which is a data visualization that displays multiple circles (bubbles) in a two-dimensional plot.

Heat map, which is a graphical representation of data where values are depicted by color.

## Outlier Detection: 
EDA involves identifying outliers within the data—anomalies that deviate significantly from the rest of the data. Tools such as box plots, z-score analysis, and scatter plots help in detecting and analyzing outliers.

## MISSING VALUE
https://www.analyticsvidhya.com/blog/2021/10/handling-missing-value/

There are three types of missing values : 
1. Missing Completely At Random(MCAR)
2. Missing At Random (MAR)
3. Missing Not At Random (MNAR)

### How to Handle Missing Data?

Missing data is a common headache in any field that deals with datasets. It can arise for various reasons, from human error during data collection to limitations of data gathering methods. Luckily, there are strategies to address missing data and minimize its impact on your analysis. Here are two main approaches:

Deletion: This involves removing rows or columns with missing values. This is a straightforward method, but it can be problematic if a significant portion of your data is missing. Discarding too much data can affect the reliability of your conclusions.
Imputation: This replaces missing values with estimates. There are various imputation techniques, each with its strengths and weaknesses. Here are some common ones:
Mean/Median/Mode Imputation: Replace missing entries with the average (mean), middle value (median), or most frequent value (mode) of the corresponding column. This is a quick and easy approach, but it can introduce bias if the missing data is not randomly distributed.
K-Nearest Neighbors (KNN Imputation): This method finds the closest data points (neighbors) based on available features and uses their values to estimate the missing value. KNN is useful when you have a lot of data and the missing values are scattered.
Model-based Imputation: This involves creating a statistical model to predict the missing values based on other features in the data. This can be a powerful technique, but it requires more expertise and can be computationally expensive.pen_spark.


### ITerative Imputer
Let’s see how IterativeImputer works. For all rows in which ‘Age’ is not missing, sci-kit learn runs a regression model. It uses ‘Sib sp’ and ‘Fare’ as the features and ‘Age’ as the target. And then, for all rows for which ‘Age’ is missing, it makes predictions for ‘Age’ by passing ‘Sib sp’ and ‘Fare’ to the training model. So it actually builds a regression model with two features and one target and then makes predictions on any places where there are missing values. And those predictions are the imputed values. as shown in MissingValue_ArticleFollowUp 

## Data Transformation 
https://www.geeksforgeeks.org/data-transformation-in-machine-learning/

Outlier : A data point which is significantly different in value from the rest of the dataset. 

Week3 Day 5 : 

Scikit - Optimize for Hyparameter Tuning in Machine Learning : 

Hyperparamter optimization refers to performing a search in order ot discover the set of specific model configuration arguments that result in the best performance of the model on a specific dataset. 

Scikit-Optimize, or skopt for short, is an open-source Python library for performing optiization tasks. 

It offers efficient optimization algorithms, such as Bayesian Optimization, and can be used to find the minimum or maximum of arbitrary cost functions. 

Bayesian Optimization provides a principled technique based on Bayes Theorem to direct a search of a global optimization problem that is efficient and effective. It works by building a probabilistic model of the objective function

Week 3 Day 6 : 

Regularization : 

Regularization is a technique used in machine learning ot prevent overfitting. OVerfitting happends when amodel learns the training data too well, including the noise and outliers, which causes it to perform poorly on new data. In simple terms, regularization adds a penalty to the model for being too complex, encoraging it to stay simpler and more general. Thsi way, it's less likely to make extreme predicitons based on the noise in the data. 

There primarily exist 3 types of Regularization : Lasso(L1), Ridge(L2) and Elastic Net(L1-L2) regularizations. The only differnece amongst them is what kind of penalty term is added. 

1. Lasso Regression : 

A regression modle which uses the L1 regularization technique is called LASSO(Least Absolute SHrinkage and Selection Operator) regression. Lasso Regression adds the "absolute value of magnitude" of the coefficient as a penalty to the loss function (L). Lasso regression also helps us achieve feature selection by penalizing the weights to approzimately equal to zero if that feature does not serve any purpose in the model 
    $$\text{Cost} = \frac{1}{n} \sum_{i=1}^{n} (y_i - \hat{y}_i)^2 + \lambda \sum_{i=1}^{m} |w_i|$$


2. Ridge Regression 

Ridge Regression adds the "squared magnitude" of the coeffecients as a penalty term to the loss function(L)
    $$\text{Cost} = \frac{1}{n} \sum_{i=1}^{n} (y_i - \hat{y}_i)^2 + \lambda \sum_{i=1}^{m} |w_i|^2$$


## Week 3 Day 7 : 

### Locally weighted regression : 

"Paramtric" learning algorithms - Fit fixed set of parameters ( $$\theta_i$$) to data 

"Non paramtric" learning algorithms - Amout of data/parameters you need to keep grows ( linearly ) with size of data. 

Skipped Part : https://www.youtube.com/watch?v=het9HFqo1TQ

Locally Weighted Regression : 

cs229 notes page 19 for detailed notes

Fit theta to minimize : 
      $$\sum_{i=1}^mw_i(y^i - \theta^TX^i)^2$$
       $$w_i = e^{-(x_i - x)/2}$$
    
https://www.geeksforgeeks.org/understanding-logistic-regression/ 

### Multinomial Logistic Regression



 