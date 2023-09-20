# APS-Prediction

The collection is made up of information gathered from large Scania vehicles in regular use. The system under consideration is the Air Pressure System (APS), which creates pressured air used for various truck operations like braking and gear changes. Component failures for a certain APS system component make up the datasets' positive class. Trucks in the bad class have malfunctions for parts unrelated to the APS. An expert-selected subset of all accessible data makes up the data.

1. After analyzing the Data it was possible to notice a large presence of missing values and how imbalanced my target variable is.
2. Before working with my missing values, my Data had 170 strings and 1 int64.
3. In my first phase of missing data cleaning, I removed all columns and rows with more than 70% missing values. Right after that, I realized that my features were skewed to the right and replaced the rest of NaN by the median.
4. After cleaning, I was left with 161 features and 57107 lines.
5. I balanced my target variable using SMOTE and normalised using Scaling and applied the machine learning algorithm to compare it with my post-PCA accuracy. Accuracy: 0.992550549840369
6. After applying the PCA and generating the variance plot, I observed that only 2 columns were needed, as they contained 99.5% of the variance.Transformed Shape (after PCA): (57107, 3)
7. After applying PCA and Machine Learning algorithms (to predict), I got an accuracy only 1% lower than before (0.9808264752232534).
8. Correctly predicted that the problems are not related to APS.
9. In summary, I have a smaller dataset to work with and less space to occupy.
