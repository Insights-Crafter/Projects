This is a machine learning model trained using weather data collected over 10 years in different cities of Australia
As a data scientist, we had to create a model that predicts rain the next day based upon the weather data collected of a particular day
For this project, Logistic Regression algorithm was used for classification the possibilty of rain tommorow as 'yes' or 'no'. The library used for machine learning is ScikitLearn (Python)
The data has alot of null values and required extensive preprocessing.
For preprocessing (includes filling the null values), built in classes of ScikitLearn library were used, namely SimpleImputer , MinMaxScaler, OneHotEncoder

Cross-Validation Accuracy: 84.84%

On average, during training with multiple data splits, your model predicted correctly about 85 times out of 100.

This checks how stable the model is across different subsets of data.

Validation Accuracy: 84.65%

When tested on a separate “validation” set (not used for training), the model still got about 85% of predictions correct.

Shows the model is not overfitting badly.

Test Accuracy: 84.78%

On the final “real-world simulation” test set, the model correctly predicted about 85% of the cases.

This is very close to training and validation results — a good sign of consistency.

Confusion Matrix:

[[21500  1172]
 [ 3255  3165]]


Interpretation:

True Negatives (TN): 21,500 → These were negative cases and the model correctly predicted them as negative.

False Positives (FP): 1,172 → These were negative cases but the model wrongly predicted them as positive.

False Negatives (FN): 3,255 → These were positive cases but the model wrongly predicted them as negative.

True Positives (TP): 3,165 → These were positive cases and the model correctly predicted them as positive.
