# Sampling-Methods

## Balancing the Dataset
To balance the above dataset, we have used SMOTE (Synthetic Minority Oversampling Technique) from the ```imblearn.over_sampling``` library.

## Defining The Sample Process
![Alt text](https://cdn.scribbr.com/wp-content/uploads/2019/09/population-vs-sample-1-300x265.png)  
Sampling is the selection of a subset of individuals from within a statistical population to estimate characteristics of the whole population.

## Types  Methods of Sampling
There are majorly two types of sampling methods
* Probabilty Sampling  
    Involves random selection process, in order  to make strong statistical inferences about the population

* Non- Probability Sampling  
    Involves non-random selection, based on convinience

Here, we will discuss about Probabilty Sampling methods

We have used five probability sampling methods on five different classification models and have compared its accuracy.

## The Five Methods of Sampling

![Alt text](https://cheggwriting.wpengine.com/wp-content/uploads/2021/11/1703-Sampling-methods-2.png)


* Simple Random Sampling  
    N number of samples are selected from the whole population, with equal probability of selection of each sample

* Stratified Sampling  
    Here, we divide the whole population into a sub-population, on the basis of some criteria or parameter. This method ensures that every group of the population is included in the sample

* Cluster Sampling  
    First, we divide the whole population into clusters of size ```N``` , then select ```n``` random clusters from the generated clusters. Here, each subgroup has similar characterics to the whole sample

* Systematic Sampling  
    Here, samples are selected from the population with a regular interval between samples.

* Multistage Sampling  
    This method of sampling is similar to stratified sampling, but here the final sample is selected from the stratified sub sample selected from the population

## Models Used

* Random Forest
* Light GBM
* XGBoost
* Logistic Regression
* Support Vector Machine

See,  ```sampling.ipynb``` for the application of the given sampling methods on the given model.



## Accuracy Report
Following is the accuracy report
![accuracy_report](https://user-images.githubusercontent.com/89384618/219968750-04d75e4a-5aa8-4454-816a-9bff1dbe905d.png)

## Conclusion  
![accuracy_report2](https://user-images.githubusercontent.com/89384618/219969060-307c0b42-6fff-4deb-b89e-a89660e6f94e.png)

From the given report, we can conclude that Cluster Sampling on the Random Forest model has the highest accuracy. Also, Random Forest performs better on any sampling method than any other model, without hyperparameter tuning.

