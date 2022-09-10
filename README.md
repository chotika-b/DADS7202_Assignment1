# Body signal of smoking 🚬
Performance comparison between traditional machine learning and deep learning.

## Discussion
1 Feature selection using feature importance

After cleaning data and doing exploratory data analysis, our group decided to finding that which features to choose for training model. Hence, feature importance is the method that we used for decision.

Using feature importance by choosing 17 features that has more influence to target variable, features that has feature importance score more than 0.03 . The result after model training on test dataset as you can see in section 7.1, using feature selection give the more accuracy and recall score. Hence, for traditional ML and MLP, we will select these 17 features for training model.

2 Imbalanced data handling

As you can see in section 5.2, The target variable between smoking and non-smoking is not balance. The non-smoking group is 63.27 % of overall record. So we used undersampling technique to handle with imbalance data and used another accuracy measurement as Recall which is more suitable measurement in this case.

As you can see in section 7.2, after train model and test, the result of model that trained after imbalanced data handling with undersampling data is giving more recall score. Therefore our project will using undersampling technique to sampling data form overall dataset.

3 Comparison result between Traditional ML and MLP

Our hypothesis before start this homework are

Tradition ML Classifier can predict whether subject is smoking or not more accuracy than MLP Classifier.
Traditiona ML will have less process time than MLP.
As a result in section 7.3, the table shows the most accurate traditional ML algorithm is ExtraTreesClassifier with 90.89 ± 0.42 which is the most accurate model among Traditional ML and MLP which go along with our assumption. Secondly, the least processing time is ExtraTreeClassifier with 3.63 seconds, and all of traditional ML has less processing time than MLP which has 13.10 seconds to finish processing.

The reason behind the result might be because this dataset has only 55,692 records, which is considered too small to use MLP. and the other reason is traditional ML is suitable for classification in this case. Not only it has more accurate result, but also has less processing time.


## Summary:
1. For this task, Traditional ML model is better than MLP, and we look at the Traditional ML result, the best Traditional ML is ExtraTreesClassifier (90.89 ± 0.42), 3.63 sec time but MLP (58.63 ± 1.65), 13.10 sec. The model that achieves state-of-the-art performance depends on the problem, available datasets. So a comprehensive comparison between traditional ML models and deep neural networks is not appropriate for this website, because it requires a lot of time and space.
2. The best Traditional ML is ExtraTreesClassifier (90.89 ± 0.42), 3.63 sec time and XGBClassifier (90.28 ± 0.13), 1.87 sec.
3. Recall score of data with feature is better than with no features selection process but a little.
4. Data show different method of dealing with unbalanced dataset like smoking and non-smoking. Use undersampling technique method to handle. The response variable can lead to better than no imbalanced data.

## Introduction
Smoking has been proven to negatively affect health and complex behavior. This project is binary classification task, classify the presence or absence of smoking through bio-signals.
dataset = https://www.kaggle.com/datasets/kukuroo3/body-signal-of-smoking


## Citing

if you find this library useful for your research. This project use this data [body-signal-of-smoking](https://www.kaggle.com/datasets/kukuroo3/body-signal-of-smoking).

    @inproceedings{plummerCITE2018,
	Author = {Nidchapan N., Prapatsorn T., Chotika B., Juthamas P., Naliya M.},
	Title = {Body signal of smoking},
	Booktitle  = {The European Conference on Computer Vision (ECCV)},
	Year = {2022}
    }

## Group members
1. 6310412022 (40%) review & MLP and result
2. 6310412024 (15%) review & Tradition ML and Conclusion
3. 6410422007 (15%) review & Data exploration after cleaning data and Discussion
4. 6410422022 (15%) review & Correlation & Feature selection
5. 6410422030 (15%) review & imbalanced data preparation

This project is a part of subject DADS7202. Data Analytics and Data Science. NIDA