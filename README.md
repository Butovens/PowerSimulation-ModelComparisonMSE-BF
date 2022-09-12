# This is an example of power simulation and Model comparison using MSE and Bayes Factor

## 1- Power simulation
Imagine that we are planning a study of how time spent observing a picture is related to how likely people are to remember the picture. We plan to randomly assign participants to view a picture for different amounts of time (10, 20, 30, 40, 50 or 60 seconds) and then have them do a memory test where they see previously studied pictures and foils and have to say if they remember each one or not. We are going to use logistic regression to analyze the data. The hypothesis is that each additional second spent studying a picture will increase the odds of remembering the picture by 1.05 times. How many subjects should we run in order to have 80% power to detect an effect corresponding to this hypothesis?

Based on some norming data, when participants have spent 0 time looking at the picture, the odds of remembering the picture are 0.42 (i.e. intercept estimate.)

## 2- Model comparison: MSE
In the **rts.csv** data set we are interested in predicting RTnaming from a variety of predictors. Using a restricting number of variables, we wil test a series of increasingly complex models, using leave-one-out cross-validation to obtain average mean-squared errors (MSEs) for training and test data sets.

## 3- Model comparison: Bayes Factor
We will use a Bayes factor analysis to probe whether there is evidence to support a model with an interaction over a simpler model (using the entirety of the **rts.csv** data set).