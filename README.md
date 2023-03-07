# Pump_sensor_project

Problem Statement

* Context
  * I have a friend who working in a small team that taking care of water pump of a small area far from big town, there are 7 system failure in last year. Those failure    cause huge problem to many people and also lead to some serious living problem of some family. The team can't see any pattern in the data when the system goes down,      so they are not sure where to put more attention.
  * Since I believe in using data to solve problem, I ask him to provide available sensor data and hope that someone here can help.

* Content
The data are from all available sensor, all of them are raw value. Total sensor are 52 unit.

* Inspiration
I hope that we can predict next failure before it's happen

We tried to build a model to predict the next failure before it happens.
* The distribution of classes in the dependent variable is imbalanced. In total 7 are broken, 14477 are recovering  and 205836 are normal.
*  After analyzing the dataset, we saw that the distribution of variables is skewed, that there are outliers, and that there is no linearity. We analyzed the variables for missing data, and because the variables there are missing less than 0.4% data, each imputer worked well. We also analyzed scaling.
* We removed empty variable and variables that correlate well with feature selection and 7% of the sensors above are missing data. Also, 'timestamp' and 'Samplenr' variables were deleted.
* We prepared data and created a window for time series.
* Trained the model with various hyperparameters, metrics and found that the best model is Support Vector Classifier.
* The worst model is MultinomialNB.
