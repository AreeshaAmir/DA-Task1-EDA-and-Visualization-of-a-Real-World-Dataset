# Data-Science-Task1
here's a summary of the insights gained:
The code begins by loading the Titanic dataset and provides initial information about its structure, data types, and the presence of missing values.
The EDA identified missing values in the 'Age', 'Cabin', and 'Embarked' columns. 'Age' was filled with the median, 'Embarked' with the mode, and 'Cabin' was dropped due to a high number of missing entries.
The code checked for and removed any duplicate rows present in the dataset, ensuring data integrity. Outliers in the 'Age' and 'Fare' columns were addressed using the Interquartile Range (IQR) method. Values falling outside the defined IQR boundaries were capped to these boundaries, mitigating the influence of extreme values. Additionally, the 'Fare' column underwent a log transformation to reduce its skewness, likely caused by a wide range of ticket prices.
The bar charts visualize the distribution of passengers across key categorical features:
  Survived: Shows the proportion of passengers who survived and those who did not.
  Pclass: Illustrates the number of passengers in each passenger class (1st, 2nd, 3rd).
  Sex: Depicts the gender distribution of the passengers.
  Embarked: Shows the number of passengers who embarked from each of the three ports.
 The histograms provide insights into the distribution of numerical features:
  Age: Shows the distribution of passenger ages after imputation and outlier handling.
  Fare: Illustrates the distribution of ticket fares after capping and log transformation.
  SibSp: Shows the distribution of the number of siblings/spouses aboard.
  Parch: Depicts the distribution of the number of parents/children aboard.
The heatmap displays the pairwise correlations between the numeric features. This helps in understanding the linear relationships between variables. For instance, it might show a correlation between passenger class and fare, or between the number of family members aboard (SibSp and Parch) and other factors. The direction and strength of these correlations can be observed from the heatmap.
The boxplots for 'Age' and 'Fare' after outlier handling visually confirm the effect of the capping process, showing a reduction in the length of the whiskers and the absence of extreme outliers.
