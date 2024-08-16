
# Reporducibility design patterns

## Transform

The problem is that the inputs to a machine learning model are not the features that
the machine learning model uses in its computations. In a text classification model,
for example, the inputs are the raw text documents and the features are the numerical
embedding representations of this text. 

The solution is to explicitly capture the transformations applied to convert the model
inputs into features.

## Repeatable Splitting

The reason is that it is rare that the rows are independent. For example, if we are training a model to predict flight delays, the arrival delays of flights on the same day will be highly correlated
with one another.

## Bridge Schema

## Windowed Inference

## Feature Store

## Model versioning






