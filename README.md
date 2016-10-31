# Feature-Selection
Dimensionality reduction techniques currently available and used in the data analytics landscape.

## Missing Values Ratio.
Data columns with number of missing values greater than a given threshold can be removed. The lower the threshold, the more aggressive the reduction.
## Low Variance Filter. 
All data columns with variance lower than a given threshold are removed. 
## High Correlation Filter. 
Calculate the correlation coefficient between numerical columns and between nominal columns as the Pearson’s Product Moment Coefficient and the Pearson’s chi square value respectively. Pairs of columns with correlation coefficient higher than a threshold are reduced to only one. 
## Random Forests / Ensemble Trees. 
Decision Tree Ensembles, also referred to as random forests, are useful for feature selection in addition to being effective classifiers.  One approach to dimensionality reduction is to generate a large and carefully constructed set of trees against a target attribute and then use each attribute’s usage statistics to find the most informative subset of features.  
## Principal Component Analysis (PCA). 
Principal Component Analysis (PCA) is a statistical procedure that orthogonally transforms the original n coordinates of a data set into a new set of n coordinates called principal components. As a result of the transformation, the first principal component has the largest possible variance; each succeeding component has the highest possible variance under the constraint that it is orthogonal to (i.e., uncorrelated with) the preceding components. Keeping only the first m < n components reduces the data dimensionality while retaining most of the data information, i.e. the variation in the data. 
## Backward Feature Elimination. 
At a given iteration, the selected classification algorithm is trained on n input features. Then we remove one input feature at a time and train the same model on n-1 input features n times. The input feature whose removal has produced the smallest increase in the error rate is removed, leaving us with n-1 input features. The classification is then repeated using n-2 features, and so on. Each iteration k produces a model trained on n-k features and an error rate e(k). 
## Forward Feature Construction. 
This is the inverse process to the Backward Feature Elimination. 
