# Credit_Risk_Analysis

## Overview of the analysis: Explain the purpose of this analysis.

This project using machine learning model to solve the risk to real-world challenge: credit card risk.

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. The feature of data is imbalanced data and we evaluate three machine learning models by using resampling to determine which is better at predicting credit risk.  By comparing different models, we will make a written recommendation on whether these models should be used to predict credit risk. 
In the given data, loan_status is as target and the rest of the 86 parameters are as dependent vaiables for using predict loan status.
## Results: Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.
preparation step includes checking missing data, null data and change data type into numeric in order to model recognize.
first model is simple random  oversampling using RandomOverSample mode . The accuracy is 68% (raw value=0.6765467429817389). Model 1 could  68% correctly predict credit card risk.

![Alt img](images\cls_report_randomoversample.png)

Second Model is  SMOTE sampling.The balance accuracy scor was 0.6419032044543083. It means that 64% data can correctly predict credit5 card risk.

![Alt img](images\cls_smote.png)

Third model is about UnderSampling where the balance accuracy is about 0.6422764227642277. It is almost the same as Smoteoversampling model.

![Alt img](images\undersampling.png)

Fourth model is combination of under and over sampling. The balance accuracy is about 0.6664102038939281. It is better than under or Smoteover sampling.

![Alt img](images\combinationsampling.png)

Fifth model is using ensamle in build fucntion in which we used the Balanced Random Forest Classifier model anmd teh balance accuracy is about 0.6830221521918328. The model has better coverage about the data. compared to the previous four models.

![Alt img](images\balanceRandomForestclassifier.png)

Model six is about Easy Ensemble AdaBoost Classifier. The balance accuracy is about 0.9316600714093861. 93 % data can be explaide by the model. It the best mode among six of them.

![Alt img](images\easyAdaBoostmodel.png)

## Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.

even though all models can predict or covered data by over 64-93% the easy Ensamble AdaBost classifier is the best among these models since it had higher 93 % of covered by the data. higher correct predictions. In addition the data is very wide range such as interest rate is very small and loan mortgae is huge values. I will suggest using the MinMaxScale methods could help the data normolized in teh same scale range.