# Linear Regression

## What is scikit learn?

Scikit learn is a powerful Python module for machine learning. It has functions for  regression, classification, clustering, model selection and dimensionality reduction.

## Step 1

Import the required Python libraries. These include numpy, pandas, scipy.stats, and matplotlib.pyplot.

## Step 2

Convert the raw data into a pandas frame, replacing the column headings if necessary.

## Step 3

Set up your variables for the predictive logic. The Y axis will usually act as the variable the model is trying to predict, while the X axis will act as the independent variable, housing all the other features

This setting up is done by importing linear regression from sci-kit learn module. Then, drop whatever variable from the data set that you would like to predict. If you want to predict the cost of housing in a certain are, drop the cost variable.

## Step 4

Store the linear regression object in a variable. Once doing so, you can then look inside of an object which will give you a list of functions available to you. Some important functions to keep in mind (this is assuming that you named the linear regression model lm):

* lm.fit() Fits a linear model

* lm.predict() Gives a prediction of Y using the linear model with estimate coefficients

* lm.score() Return the coefficient  of determination (R^2).This is a measure of how well the observed outcomes of the actual data are replicated by the model

* .coef_ gives the coefficients

* .intercept_ gives the estimated intercepts

## Fitting a linear model

Construct a dataframe with the independent features and the estimated coefficients of the data set.

You can then create a scatter plot with the predicted values given the features.

You can then create a scatter plot checking those values against the actual values of the variable. When you do this you can calculate a mean square error.

Mean square error: A measure of how close the prediction was to the actual.

In practice when machine training, give the model set of data rather than the entire set. This will ensure that you train your model on training data so that you can then see how well ir performs on the test data.

## Residual Plots

Residual plots are a way to visualize how well the prediction did against the actual data set. If within a residual plot there seems to be a patter emerging, rather than a random scattering of points through the set, then you have a relationship between variables wrong. This means that you should go back to the model and change something about the parameters.
