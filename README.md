**Title – Fault Detection in Thermal Storage Insulation**

**About -** Predict anomaly in thermal storage insulation system on the basis of dataset containing readings of thermal sensors and pressure sensors.

**Supervised Machine Learning Project –** It has labeled data or simply we can say that we have output column ‘anomaly’ to predict. 

1. **Data Import** – The dataset is downloaded from Kaggle which is in CSV format.

1. **EDA** – 
1. Finding all variables and understand them
1. cleaning data set (null values, un-necessary columns,)
1. Identify co-related values
1. Univariate Analysis (non graphical) – find out central tendency, range, variance and standard deviation 
1. Univariate Analysis (graphical) – simple bar charts, multiple or grouped charts,   percentage bar charts, box plot
1. Multivariate chart – scatter plot, heat map

1. **Data Transformation –** converting the data into the suitable format for analysis.** Data is transformed to make it better organized. Transformed data may be easier for both humans and computers to use. Properly formatted and validated data improves data quality 
1. Normalization - Normalization is used to scale the data to a common range. This method scales the model using minimum and maximum values. Values on the scale fall between [0,1] and [-1,1]
1. Standardization - standardization is used to transform the data to have zero mean and unit variance. This method scales the model using the mean and standard deviation. Values on a scale are not constrained to particular range.
1. Discretization - Discretization is used to convert continuous data into discrete categories.
1. get\_dummies – for categorical values

1. **Train test split –** splitting** the dataset in two parts training (80%) and testing (20%) 

1. **Algorithms –** 
1. **Logistic Regression –** 
- It is used when the dependent variable is binary (0/1, True/False, Yes/No) in nature. Logistic regression is a classification algorithm used to find the probability of event success and event failure. 
- The major limitation of Logistic Regression is the assumption of linearity between the dependent variable and the independent variables. (if the data points can be separated using a line, linear function, are considered linearly separable.)
- Generally, the closer a correlation coefficient is to 1.0 (or -1.0) the stronger the relationship between the two variables is said to be.
- For this dataset ‘Logistic Regression’ gives **66.56%** accuracy.

1. **Decision Tree Classifier –** 
- In this case Decision Tree Classifier gives us better result than logistic regression **(94%)**. 
- Here we get better results than ‘Logistic Regression’ because **Decision Boundaries** (the lines that are drawn to separate different classes). Decision Tree bisect the space into smaller regions, whereas Logistic Regression fits a single line to divide the space exactly into two.
- In case of Logistic Regression a decision thresholds to be set and in Decision Tree it automatically handles decision making

1. **Random Forest Classifier –**
- A random forest is a meta estimator that fits a number of decision tree classifiers on various sub-samples of the dataset and uses averaging to improve the predictive accuracy and control over-fitting. 
- Random Forest is a tree-based machine learning algorithm that leverages the power of multiple decision trees for making decisions. As the name suggests, it is a “forest” of trees!
- Random forest leverages the power of multiple decision trees. It does *not* rely on the feature importance given by a single decision tree.
- Random Forest Classifier gives us **(95%)** of accuracy.




1. **Boosting Algorithms –** 

Boosting is one of the techniques that use the concept of ensemble learning (Ensemble learning is an approach in which two or more models are fitted to the same data, and the predictions of each model are combined.). A boosting algorithm combines multiple simple models (also known as weak learners or base estimators) to generate the final output.

1. **Gradient Boosting Machine (GBM) –** 
- A Gradient Boosting Machine or GBM combines the predictions from multiple decision trees to generate the final predictions.
- All the weak learners in a gradient boosting machine are decision trees.
- Gradient boosting gives us **(88%)** accuracy.
1. **Extreme Gradient Boosting Machine (XGBM) –** 
- To improve results we use XGBoost algorithm. XGBoost also includes a variety of regularization techniques that reduce overfitting and improve overall performance. 
- XGBoost gives us **(96.82%)** accuracy.


