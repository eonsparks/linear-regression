## Simple Linear Regression

Simple linear regression is a statistical method that allows us to summarize and study relationships between two continuous variables:
- One variable, denoted as X, is regarded as the predictor, explanatory, or independent variable.
- The other variable, denoted as Y, is regarded as the response, outcome, or dependent variable.

### Concept

The goal of simple linear regression is to find a linear function that predicts the dependent variable (Y) as accurately as possible as a function of the independent variable (X).

### Mathematical Representation

The simple linear regression model can be represented by the equation:

Y = β₀ + β₁X + ε

Where:
- Y is the dependent variable
- X is the independent variable
- β₀ is the y-intercept (the value of Y when X = 0)
- β₁ is the slope (the change in Y for a unit change in X)
- ε is the error term (the difference between predicted and actual Y values)

### Estimating Parameters

To find the best-fitting line, we need to estimate β₀ and β₁. This is typically done using the method of least squares, which minimizes the sum of squared residuals.

The formulas for β₀ and β₁ are:

β₁ = Σ((X - X̄)(Y - Ȳ)) / Σ((X - X̄)²)
β₀ = Ȳ - β₁X̄

Where X̄ and Ȳ are the means of X and Y respectively.

### Implementation Approach

1. Data Preparation:
   - Load the dataset
   - Split into X (independent) and Y (dependent) variables

2. Calculate Statistics:
   - Compute means of X and Y
   - Compute the sum of squares for X and XY

3. Compute Parameters:
   - Calculate β₁ (slope) using the formula above
   - Calculate β₀ (intercept) using the formula above

4. Make Predictions:
   - Use the equation Y = β₀ + β₁X to predict Y for any given X

5. Evaluate the Model:
   - Calculate residuals (differences between actual and predicted Y values)
   - Compute R-squared (coefficient of determination) to assess model fit

6. Visualize Results:
   - Plot the original data points
   - Plot the regression line

This approach can be easily translated into code using libraries such as NumPy for calculations and Matplotlib for visualization.
