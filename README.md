# Credit_Risk_Analysis
## Overview of the analysis:
In this analysis, I applied machine learning to solve a real-world challenge: credit card risk.

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, I will need to employ different techniques to train and evaluate models with unbalanced classes. I used imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersampled the data using the ClusterCentroids algorithm. Then, I used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, I compared two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Lastly, I evaluated the performance of these models and made a written recommendation on whether they should be used to predict credit risk.

## Results: Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.

**- Naive Random Oversampling:**
  - The balanced accuracy score is about 65%
  - The high risk precision score is about 1% with 62% sensitivity
  - The low risk precision score is 100% with 68% sensitivity

<img width="930" alt="Screen Shot 2021-12-02 at 9 40 44 PM" src="https://user-images.githubusercontent.com/88408350/144551481-1dc675fe-dc34-456a-b15e-b6b408269547.png">
<img width="733" alt="Screen Shot 2021-12-02 at 9 40 52 PM" src="https://user-images.githubusercontent.com/88408350/144551504-56a801d1-5a16-4bc8-802f-83f7cb2ad38e.png">


**- SMOTE oversampling results:**
  - The balanced accuracy score is about 64%
  - The high risk precision score is about 1% with 63% sensitivity
  - The low risk precision score is 100% with 66% sensitivity

<img width="929" alt="Screen Shot 2021-12-02 at 9 46 22 PM" src="https://user-images.githubusercontent.com/88408350/144551982-b6006070-1a60-4374-af81-5d9cec063861.png">
<img width="723" alt="Screen Shot 2021-12-02 at 9 46 28 PM" src="https://user-images.githubusercontent.com/88408350/144551989-43c45975-e288-43ba-a623-3efddb26c694.png">


**- ClusterCentroids:**
  - The balanced accuracy score is about 53%
  - The high risk precision score is about 1% with 61% sensitivity
  - The low risk precision score is 100% with 45% sensitivity

<img width="931" alt="Screen Shot 2021-12-02 at 9 49 58 PM" src="https://user-images.githubusercontent.com/88408350/144552344-12602efb-0651-454e-b704-cea7167e1b58.png">
<img width="712" alt="Screen Shot 2021-12-02 at 9 50 04 PM" src="https://user-images.githubusercontent.com/88408350/144552351-22d98be2-1041-4ebf-997c-fafdc0f499f2.png">

**- SMOTEENN:**
  - The balanced accuracy score is about 62%
  - The high risk precision score is about 1% with 68% sensitivity
  - The low risk precision score is 100% with 57% sensitivity

<img width="929" alt="Screen Shot 2021-12-02 at 9 52 40 PM" src="https://user-images.githubusercontent.com/88408350/144552584-9b0786ab-4949-4258-9896-d158479a28c9.png">
<img width="730" alt="Screen Shot 2021-12-02 at 9 52 47 PM" src="https://user-images.githubusercontent.com/88408350/144552599-6396da53-fac7-4ed9-983c-9bd453d56a22.png">


**- Balanced Random Forest Classifier:**
  - The balanced accuracy score is about 79%
  - The high risk precision score is about 4% with 67% sensitivity
  - The low risk precision score is 100% with 91% sensitivity

<img width="937" alt="Screen Shot 2021-12-02 at 9 54 21 PM" src="https://user-images.githubusercontent.com/88408350/144552730-72a9da40-11a6-4dd9-a4e8-a171ed28cc50.png">
<img width="733" alt="Screen Shot 2021-12-02 at 9 54 28 PM" src="https://user-images.githubusercontent.com/88408350/144552741-ba9bc8ee-387f-4135-93dc-72c06391dc6a.png">

**- Easy Ensemble AdaBoost Classifier:**

## Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning
