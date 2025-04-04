Task 1:
Problem statment:Implement a linear regresson model to predict the price of house based on their square footage and the number of bedrooms and bathrooms.
Provided dataset:https://www.google.com/url?q=https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data&sa=D&source=editors&ust=1743753434222486&usg=AOvVaw14dWvQCwVJ68w7FSPIyKUg
learnings about linear regression:

1. **Overview of Linear Regression**: 
   - Linear regression aims to find a straight line (or more generally, a plane or higher-dimensional model) that best fits a dataset.
   - The goal is to predict one variable based on another. In the example provided, the data concerns predicting the **mouse size** based on **mouse weight**.

2. **Fitting a Line to Data**:
   - **Least Squares Method** is used to find the best-fitting line, which minimizes the sum of squared residuals (the vertical distance between data points and the line).
   - **Residuals**: The differences between the observed data points and the predicted values on the line. The goal is to minimize the sum of squared residuals to find the best-fit line.

3. **R-squared (R²)**:
   - **R²** measures how well the model explains the variation in the data. It ranges from 0 to 1, where:
     - **0** means the model explains none of the variance.
     - **1** means the model explains all the variance.
   - A value like **0.6** means 60% of the variation in the data can be explained by the independent variable (in this case, mouse weight).

4. **Calculating R-squared**:
   - The video demonstrates how to calculate R² using the sum of squares:
     - **Total Sum of Squares** (SS_total): The variation in the dependent variable (mouse size) relative to the mean of the data.
     - **Sum of Squares for the Fit** (SS_fit): The variation explained by the model (after fitting the line).
     - **R² = (SS_total - SS_fit) / SS_total**.

5. **Multivariable Regression**:
   - The video expands on how linear regression can be used for models with multiple variables (e.g., predicting mouse body length based on weight and tail length).
   - In this case, the model fits a plane instead of a line in a 3D space (because we have three variables), and the concept of R² can be applied similarly.

6. **Adjusted R-squared**:
   - **Adjusted R²** adjusts R² for the number of parameters in the model. Adding more variables to a model can artificially increase R², even if the new variable doesn't really explain much. The adjusted R² helps mitigate this by penalizing unnecessary complexity.

7. **P-value for R-squared**:
   - The **p-value** helps determine if the observed relationship is statistically significant. A p-value can be calculated based on an F-test, which compares the variance explained by the model to the unexplained variance.
   - A lower p-value indicates that the model is statistically significant and that the relationship between the variables is not due to random chance.

**Main Concepts Covered**:
- **Least Squares**: Used to find the best-fitting line.
- **Residuals**: Measure the error in predictions.
- **R-squared**: Tells us how well the model fits the data.
- **Multivariable Models**: Explains how adding more variables can increase the complexity of a model (and the R² value).
- **P-value**: Used to assess the statistical significance of the model.
