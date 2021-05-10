# Machine learning based early mortality prediction in the emergency department 

* Xiao Yu
* 2021/03/15

## Main Content

There are seven jupyter notebooks (including comments)

1. `mortality_prediction.ipynb` ：Include basic data preprocessing, as a comparison, take the max, min, median, mean, std of each time sequence vital signs as the basic features to predict the early mortality of patients.
2. `models_fine-tuning.ipynb` ：The hyper-parameters of the model were fine-tuned, including logistic regression (LR), k-nearest neighbor (KNN), gaussian naive byes (GaussianNB), support vector classification (SVC), decision tree (DT), random forest (RF), adaptive boosting (AdaBoost), gradient boosting decision tree (GBDT), light gradient boosting machine (LightGBM). 
3. `models_shap_analysis.ipynb` ：Through the shap value (a unified approach to interpreting model predictions) for model explanatory analysis.
4. `test_critical_value.ipynb` ：The features of critical variables were constructed, but the effect was not improved.
5. `feature_create_vital_signs.ipynb` ：Use the automation tool tsfresh          ([https://tsfresh.readthedocs.io](https://tsfresh.readthedocs.io/en/latest/)) to construct the time series-based features of vital signs, and test the preliminary effect.
6. `time_interval_validation_vital_signs.ipynb` ：Objective to explore the influence of different time windows on the final prediction effect of patients.
7. `nums_of_feature_comparsion.ipynb` ***(final)*** ：This paper explores the influence of the number of time series-based features on the final prediction results, as well as the cross validation, result comparison and mapping of various indicators.
