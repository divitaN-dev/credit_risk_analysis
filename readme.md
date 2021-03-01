## Overview of Project

Credit risk analysis is a common unbalanced classification problem as good loans tend to easily outnumber risky ones. This analysis deploys six machine learning models to calculate accuracy, precision and recall scores.

### Purpose

The purpose of the analysis is to implement the following machine learning models to resample data in order to create a more balanced dataset and minimise bias. 
    *Random OverSampler
    *SMOTE
    *Cluster Centroids
    *SMOTEENN
    *Balanced Random ForestClassifier
    *Easy Ensemble Classifier
    
The data is resampled uses oversampling, undersampling, combination and ensemble learning techniques to avoid overfitting where a model's predictions lean excessively to a specific dataset and provided poor predictions for new datasets.

An accuracy score, confusion matrix and classification report is generated to measure accuracy,precision and recall scores.

## Results

Definitions-
    *Precision - the reliability of a postivie classification, in this case - the reliability of a high risk loan classification.

    *Recall - the ability of a model to predict all positive outcomes, in this case - the ability to predict all high risk loan applications.

*Random Oversampler - Oversampling
    *Accuracy score - 66%
    *Precision rate - 99%
    *Recall rate - 65%

    ![random-oversampler](https://github.com/divitaN-dev/stocks-analysis-macro/blob/main/resources/stocks-analysis-2017.png)

*SMOTE Oversampler - Oversampling
    *Accuracy score - 64.3%
    *Precision rate - 99%
    *Recall rate - 65%

    ![SMOTE](https://github.com/divitaN-dev/stocks-analysis-macro/blob/main/resources/stocks-analysis-2017.png)

*Cluster Centroids - Undersampling
    *Accuracy score - 53%
    *Precision rate - 99%
    *Recall rate - 45%

    ![cluster-centroids](https://github.com/divitaN-dev/stocks-analysis-macro/blob/main/resources/stocks-analysis-2017.png)

*SMOTEENN Combination sampler - (Over and Under) sampling
    *Accuracy score - 63%
    *Precision rate - 99%
    *Recall rate - 55%

    ![SMOTEENN](https://github.com/divitaN-dev/stocks-analysis-macro/blob/main/resources/stocks-analysis-2017.png)

*Balanced Random Forest Classifier 
    *Accuracy score - 53%
    *Precision rate - 99%
    *Recall rate - 45%

    ![balanced-random](https://github.com/divitaN-dev/stocks-analysis-macro/blob/main/resources/stocks-analysis-2017.png)

*Easy Ensemble Classifier
    *Accuracy score - 92%
    *Precision rate - 99%
    *Recall rate - 94%

    ![easy-ensemble](https://github.com/divitaN-dev/stocks-analysis-macro/blob/main/resources/stocks-analysis-2017.png)


*There are a total of 15 different schools with 39,170 students.
*The total budget of all schools is - $24,649,428.
*The average reading score and percentage across the district is higher than the average math score and percentages.
*The overall passing percentage of students is 64.9%.

![district-summary](https://github.com/divitaN-dev/stocks-analysis-macro/blob/main/resources/stocks-analysis-2017.png)


### Summary

*The sampling models using over, under and combination sampling did not perform well with the credit risk dataset, although the precision rates are high, none of them performed well in terms of accuracy and recall. A high percentage of reacll is cruical in this case as the number of high risk loans are low in the overall dataset and the ability to predict all positive outcomes is non-negotiable in this scenario.

*The Easy Ensemble Classifier that employs boosting outperformed all other models with high scores in accuracy, precision and most important in our case - recall. This model would work best in analysing credit risk of loans. 