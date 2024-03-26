# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.

The purpose of this analysis is to predict loan status (paying as expected vs. in default).

* Explain what financial information the data was on, and what you needed to predict.

The financial data that was provided are several variables that are indicative of credit quality, ranging from borrower income to the number of derogatory marks on their credit bureau.

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).

The 'loan status' variable I was trying to predict is a binary variable, and only 3.2% of the observations are a '1'. That would indicate that the 1 represents a bad loan, and the 0 is a loan in good standing. There are a total of 77536 observations, of which about 2500 are bad.

* Describe the stages of the machine learning process you went through as part of this analysis.

I first split the dataset into partitions that can be used to both train and test the model. This allowed me to avoid overfitting the full dataset, and provided a more realistic assessment of model's accuracy. I then fit a logistic regression to the training partition, and predicted bad loans using that mdoel.

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

I used a logistic regression model, which allowed me to predict the log odds of a binary variable, which in this case is an indication of loan status.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.

Accuracy: 99% Precision: macro-94%, wgt 99% Recall: macro-97%, wgt 99%

* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

  INSTUCTOR TOLD THE CLASS TO OMIT THIS PORTION BECAUSE IT WAS OUTDATED.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?

NA - only had one model. However, it did perform relatively well, but it would important to test multiple different models before making a recommendation for the best to use.

* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.


Predicting good loans is less difficult as they are the majority of observations. The precision was also lower for the 'bad loan' prediction, at just 87%. Given the importance of predicting bad loans, 87% may not be sufficient for this analysis.

If you do not recommend any of the models, please justify your reasoning.

87% precision when predicting bad loans seems inadequate. It would be the recommendation that we continue to explore better models before finalizing this analysis.