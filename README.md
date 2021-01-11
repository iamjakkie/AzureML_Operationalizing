
# Operationalizing Machine Learning Model
## Overview
The objective of this repo is to go through AutoML process, deploy the best model and test endpoints.

## Dataset
Used dataset is generally available [Source](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing) and it is data gathered from direct marketing campaigns by a bank.
The goal is to predict whether the customer will subscribe for a term deposit or not, based on age, job, education etc.

## Architectural Diagram
![img](/img/operationizingarchitecture.png)

### Deployment
Deployment has been split into two different approaches:
1. Manual Deployment - in Azure ML Studio
2. Pipeline Deployment - through code in a Jupyter notebook

## Key Steps
 1. Authentication
 2. AutoML Experiment

### Dataset registration
![img](/img/dataset.PNG)
Dataset has been registered as a tabular dataset
### AutoML Experiment
![img](/img/experiment.PNG)
![img](/img/bestmodel3.PNG)
![img](/img/bestmodel2.PNG)
![img](/img/bestmodel1.PNG)
![img](/img/VotingEnsemble.PNG)

The best model found during automl was VotingEnsemble

3. Deployment
The best model has been deployed manually into ACI with authentication enabled.

4. Enable logging

![img](/img/logs.PNG)
![img](/img/appinsights.PNG)

5. Swagger

![img](/img/swagger1.PNG)
![img](/img/swagger2.PNG)

6. Consume endpoint

![img](/img/consume1.PNG)

7. Pipeline execution
