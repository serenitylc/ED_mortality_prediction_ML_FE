# Machine learning based early mortality prediction in the emergency department 

* Xiao Yu
* 2020/10/11

## 主要内容

总共包含7个 jupyter notebook (含注释)

1. `mortality_prediction.ipynb` ：包含基本数据预处理，作为对比，取每个时序生命体征的 max, min, median, mean, std 作为基本特征来预测患者早期死亡率。
2. `models_fine-tuning.ipynb` ：对模型超参数进行微调，包括         logistic regression (LR), k-nearest neighbor (KNN), gaussian naive byes (GaussianNB), support vector classification (SVC), decision tree (DT), random forest (RF), adaptive boosting (AdaBoost), gradient boosting decision tree (GBDT), light gradient boosting machine (LightGBM). 
3. `models_shap_analysis.ipynb` ：通过shap value (A Unified Approach to Interpreting Model Predictions) 作模型解释性分析。
4. `test_critical_value.ipynb` ：构建危急值特征，无效果提升。
5. `feature_create_vital_signs.ipynb` ：使用自动化工具tsfresh          ([https://tsfresh.readthedocs.io](https://tsfresh.readthedocs.io/en/latest/)) 构建生命体征时序特征，以及初步效果测试。
6. `time_interval_validation_vital_signs.ipynb` ：探究不同时间窗口对患者最终预测效果的影响。
7. `nums_of_feature_comparsion.ipynb` ***(final)*** ：探究时序特征个数对最终预测结果的影响，以及各个指标的交叉验证、结果对比、作图等。