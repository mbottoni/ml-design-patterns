
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

NaN imputation??

## Windowed Inference

## Workflow pipeline

In addition to TFX, Apache Airflow and Kubeflow Pipelines are both alternatives for
implementing the Workflow Pipeline pattern. Like TFX, both Airflow and KFP treat
pipelines as a DAG where the workflow for each step is defined in a Python script.
They then take this script and provide APIs to handle scheduling and orchestrating
the graph on the specified infrastructure. Both Airflow and KFP are open source and
can therefore run on-premises or in the cloud.

## Feature Store

Good feature engineering is crucial for the success of many machine learning solu‐
tions. However, it is also one of the most time-consuming parts of model develop‐
ment. Some features require significant domain knowledge to calculate correctly, and
changes in the business strategy can affect how a feature should be computed.

The solution is to create a shared feature store, a centralized location to store and
document feature datasets that will be used in building machine learning models and
can be shared across projects and teams

- kafka
- redis / cassandra
- hive / bigquery

- open source feature store: feast


## Model versioning






