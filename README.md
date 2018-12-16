# Machine learning lifecycle lab
A collection of notebooks for walking through the typical ML lifecycle from data cleaning through to model hosting using Amazon SageMaker.

A typical ML lifecycle will look something like...
 1. Identify a business problem or question which ML can answer
 1. Identify the data sources available to describe the problem space
 1. Acquire and cleanse the data or a sample of the data
 1. Engineer a feature set from the data or data sample so that everything has meaning and relevance
 1. Apply this cleansing and feature engineering logic to the full data set
 1. Spot check multiple ML algorithms against a sample of the feature set to assess which algorithm is likely to give the best result
 1. Select one or more algorithms and perform hyperparameter optimization to determine the best configuration parameters, use a sample of the feature set
 1. Train a model using the best performing algorithm and hyperparameters on the full training feature set
 1. Test the model on a control or test feature set to produce a baseline for performance
 1. Deploy the model for consumption by the business (Lambda, mobile device, container, etc)
   1. Consider how future observations will be engineered in preparation for inference
 1. Monitor the model for context drift
 
For this collection of labs we will start by defining a business problem and then work through the process through to model deployment.  

 
 Table of contents
 ---

 1. [Feature engineering](01 Feature engineering.ipynb)
 This notebook walks through acquiring the data, cleaning it and then engineering a base feature set which can then be prepared for ML training.
 1. [ML algorithm spot check](02 Algorithm spot check.ipynb)
 This notebook walks through transforming the cleansed data to assess the performance of many ML algorithms.
 1. [HPO and training](03 Hyperparameters and training.ipynb)
 This notebook walks through performing HPO on an algorithm and a subset of the feature set before performing a full scale training job.
 1. [Hosting and usage](04 Hosting inference.ipynb)
 This notebook walks through how to host a trained model and use it to make predictions.
 
 ## Further reading
 - [What’s your ML test score? A rubric for ML production systems](https://ai.google/research/pubs/pub45742)
 - [Automation of data profiling](https://github.com/pandas-profiling/pandas-profiling)
 - [Automated data profiling example](http://nbviewer.jupyter.org/github/JosPolfliet/pandas-profiling/blob/master/examples/meteorites.ipynb)
 - [Automated data profiling for Spark](https://github.com/julioasotodv/spark-df-profiling)
 - [Machine Learning: The High Interest Credit Card of Technical Debt](https://ai.google/research/pubs/pub43146)
