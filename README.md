## About the Project
This project mainly focused on applying deep learning models for a house price prediction problem.

### Tools used
Python - Keras / tensorflow

### Dataset

The dataset consists of attributes to predict the house price

### Data PreProcessing

* Checking null values
* Remove duplicates
* Remove unwanted variables
* Label encoding
* Scaling the data

### Model Fitting

Three models are executed in the current project.

1. Linear Regression model
2. First Keras Model: Consisting of two layers and Adam optimizer.
3. Second Keras Model: with RMSProp optimizer consists of 4 layers and the first uses 20% dropouts.

### Model Evaluation

**Linear Regression (LR) Model:**

* Mean Squared Error (MSE): 45815668513.09734
* Root Mean Squared Error (RMSE): 214045.94953676965
* Correlation between predicted and the actual values: 0.812


**Keras Model - 1 :**

* Mean Squared Error (MSE): 216763633800.68573
* Root Mean Squared Error (RMSE): 465578.8158847927
* Correlation between predicted and the actual values: 0.447

Based on the comparison of these metrics:

* MSE and RMSE Comparison: The LR model had a substantially lower MSE and RMSE compared to the Keras model. A lower MSE and RMSE indicate better predictive accuracy, with the LR model outperforming the Keras model in this regard. The LR model's predictions were closer to the actual values compared to the Keras model.

* Correlation Comparison: The LR model exhibited a significantly higher correlation between the true and predicted values (0.812) than the Keras model (0.447). A higher correlation suggests a stronger linear relationship between the predictions and actual values. The LR model's better correlation implies that it captured more of the underlying patterns in the data.

* Given the provided results and metrics, the previous Linear Regression model appears to be the better choice for predicting house prices compared to the new Keras model. The LR model displayed lower MSE and RMSE values, indicating superior predictive accuracy, and it had a higher correlation, implying a stronger relationship between predictions and actual values.

**Keras Model - 2 :** 

* Mean Squared Error: 37167669951.88608
* Root Mean Squared Error: 192789.18525655445
* Correlation between predicted and the actual values: 0.855

Based on the comparison of these metrics:

* The previous Linear Regression (LR) model yielded a Mean Squared Error (MSE) of approximately 45815668513.10 and a Root Mean Squared Error (RMSE) of 214045.95. The correlation between the true and predicted values was 0.812. On the other hand, the new Keras model produced a lower MSE of about 37167669951.89, a lower RMSE of 192789.19, and an improved correlation of 0.855.

* These results suggest that the Keras model outperforms the Linear Regression model in terms of predictive accuracy. The lower MSE and RMSE values indicate that the Keras model's predictions are closer to the actual house prices, implying better model fit. Additionally, the higher correlation signifies a stronger linear relationship between the Keras model's predictions and the true house prices, indicating a more accurate representation of the underlying data patterns.
