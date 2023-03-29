# Credit_Risk_Analysis

## Overview of the Analysis

The purpose of this review is to use supervised learning models to train and evaluate models to classify risk for credit card customers. The review will use data fromLendingClub to run several analyses to ultimately determine whether the models created can be used to predict credit risk. The data will first be split into testing and training data and then six models will be used to perform an analysis. With each model, the balanced accuracy score, precision and recall score of each model will be shown and then used later to recommend a particular model

## Results

### Resampling Techniques

The first batch of techniques is over and undersampling with the following results

### Naive Random Oversampling

![Naive Random Oversampling](https://github.com/UnBearAble1/Credit_Risk_Analysis/blob/main/Naive%20Random%20Oversampling.png)

* Balanced accuracy score: 0.64
* Precision score: 0.99
* Recall score: 0.58

### SMOTE Oversampling

![SMOTE Oversampling](https://github.com/UnBearAble1/Credit_Risk_Analysis/blob/main/SMOTE%20Oversampling.png)

* Balanced accuracy score: 0.66
* Precision score: 0.99
* Recall score: 0.68

### Undersampling

![Undersampling](https://github.com/UnBearAble1/Credit_Risk_Analysis/blob/main/Undersampling.png)

* Balanced accuracy score: 0.54
* Precision score: 0.99
* Recall score: 0.40

###Combination (Over and Under) Sampling

![Combination (Over and Under) Sampling](https://github.com/UnBearAble1/Credit_Risk_Analysis/blob/main/Combination%20(Over%20and%20Under)%20Sampling.png)

* Balanced accuracy score: 0.65
* Precision score: 0.99
* Recall score: 0.57

### Ensemble Techniques

The second group of analyses are ensemble with the following results:


### Balanced Random Forest Classifier

![Balanced Random Forest Classifier](https://github.com/UnBearAble1/Credit_Risk_Analysis/blob/main/Balanced%20Random%20Forest%20Classifier.png)

* Balanced accuracy score: 0.76
* Precision score: 0.99
* Recall score: 0.87

The Balanced Random Forest Classifier also provides scores for those features that are most important to the model. The top features based on the random forest classifier are as follows:

* total_rec_prncp: (0.06908193799083064)
* total_pymnt_inv: (0.06575569588802577)
* last_pymnt_amnt: (0.05746689911784709)
* total_pymnt: (0.05524571371644502)
* total_rec_int: (0.05173067665093821)

### Easy Ensemble AdaBoost Classifier

![Easy Ensemble AdaBoost Classifier](https://github.com/UnBearAble1/Credit_Risk_Analysis/blob/main/Easy%20Ensemble%20AdaBoost%20Classifier.png)

* Balanced accuracy score: 0.93
* Precision score: 0.99
* Recall score: 0.94

## Summary

The balanced accuracy score, or the measure of how accurate the test results were based on the training module varied widely amongst each model, ranging from 54% to 93%. none of the results seemed to be too high, meaning that the data was most likely not oversampled

The precision scores, which measure the number of true positive results by all positive results (true and false) for each test was 99%, meaning that every test was very accurate in determining which results were true and not having too many false positive results

Lastly, the recall (or sensitivity) scores for the models ranged significantly, from a low of 40% to a high of 94%. The recall score for this test measures that if a person is a credit risk, how likely is it that the test will identify them as a credit risk, so the higher the result, the more likely that credit risks are correctly identified as risks and not that credit risks are inaccurately labeled as not a credit risk

### Recommendation

Based on the results, my recommendation is the Easy Ensemble AdaBoost method. Its high precision rate of 99% means that predicted positive rates are 99% likely of being a true positive and the recall rate of 94%, the highest of all of the models, means that it has the highest rate of detecting all positive results. Lastly, its accuracy score of 93% means that it is correct 93% of the time, which is the highest result of all of the models utilized.
