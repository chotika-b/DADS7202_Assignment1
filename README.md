# Body signal of smoking 🚬
Performance comparison between traditional machine learning and deep learning.

## Summary:
1. For this task, Traditional ML model is better than MLP, and we look at the Traditional ML result, the best Traditional ML is ExtraTreesClassifier (90.89 ± 0.42), 3.63 sec time but MLP (58.63 ± 1.65), 13.10 sec. The model that achieves state-of-the-art performance depends on the problem, available datasets. So a comprehensive comparison between traditional ML models and deep neural networks is not appropriate for this website, because it requires a lot of time and space.
2. The best Traditional ML is ExtraTreesClassifier (90.89 ± 0.42), 3.63 sec time and XGBClassifier (90.28 ± 0.13), 1.87 sec.
3. Recall score of data with feature is better than with no features selection process but a little.
4. Data show different method of dealing with unbalanced dataset like smoking and non-smoking. Use undersampling technique method to handle. The response variable can lead to better than no imbalanced data.

**Table of Contents**
1. [Introduction](#Introduction)
2. [Data Preparation](#Data-Preparation)
3. [Data exploration after cleaning data](#Data-exploration-after-cleaning-data)
4. [Correlation & feature selection](#Corretion-and-Feature-Selection)
5. [Tradition ML](#Tradition-ML)
6. [MLP](#MLP)
7. [Result](#Result)
8. [Discussion](#t8.)
9. [Conclusion](#t9.)

## 1. Introduction
Smoking has been proven to negatively affect health and complex behavior. This project is binary classification task, classify the presence or absence of smoking through bio-signals.
dataset = https://www.kaggle.com/datasets/kukuroo3/body-signal-of-smoking

## 2. Data Preparation
2.1 Loading Dataset
2.2 Variables Description
2.3 Descriptive Statistics
2.4 Basic Information About Dataset
2.5 Convert data type to number

## 3. Data exploration after cleaning data
3.1 Overall category each attributes
3.1.1 Quantitative Features
3.1.2 Qualitative Features
3.2 Imbalance data

## 4. Corretion and Feature Selection
4.1 Correlation
4.2 Feature Selection by using feature importances
4.3 Data splitting and test the result between using all features ( except ID ) and feature importances selection.

## 5. Tradition ML
5.1 Split the Dataset into Train and Test Sets
5.2 Verfiy imbalanced
5.3 Random Under-Sampling
5.4 Equally Distributing and Correlating
5.5 Machine Learning Classification Algorithms
5.5.1 Non-under sampling data
5.5.2 Under sampling data

## 6. MLP
6.1 Network Architecture
6.2 Accuracy & Loss History
6.3 Result

## 7. Result
7.1 Features selection
score comparision between data with "features selection" process and "no-features selection" process
<GaussianNB> using the best model for features selection task

	data with features selection process    : recall     = 80.23 %
	data with no features selection process : recall     = 80.17 %

	data with features selection process    : accuracy   = 70.99 %
	data with no features selection process : accuracy   = 70.52 %
===================================================
score of data with features selection process is higher than data with no features selection process
features =  ['serum creatinine', 'weight(kg)', 'age', 'relaxation', 'AST', 'systolic', 'fasting blood sugar', 'HDL', 'ALT', 'Cholesterol', 'LDL', 'waist(cm)', 'triglyceride', 'height(cm)', 'Gtp', 'hemoglobin', 'gender']
number of feaures : 17

7.2 Imbalanced data preparation
score comparision between data with "imbalanced data preparation" process and "no imbalanced data preparation" process
<ExtraTreesClassifier> using the best model for imbalnced data preparation task

	data with imbalanced data preparation process    : recall = 90.89 ± 0.42 %
	data with no imbalanced data preparation process : recall = 75.16 ± 0.42 %

	data with imbalanced data preparation process    : accuracy = 79.17 ± 0.41 %
	data with no imbalanced data preparation process : accuracy = 79.41 ± 0.41 %
===================================================
score of data with imbalanced data preparation process is higher than data with no imbalanced data preparation process

7.3 Traditional ML and MLP comparision
image.png

## Citing

if you find this library useful for your research. This project use this data [body-signal-of-smoking](https://www.kaggle.com/datasets/kukuroo3/body-signal-of-smoking).

    @inproceedings{plummerCITE2018,
	Author = {Nidchapan N., Prapatsorn T., Chotika B., Juthamas P., Naliya M.},
	Title = {Body signal of smoking},
	Booktitle  = {The European Conference on Computer Vision (ECCV)},
	Year = {2022}
    }

## Group members
1. 6310412022
2. 6410422007
3. 6410422022
4. 6410422024