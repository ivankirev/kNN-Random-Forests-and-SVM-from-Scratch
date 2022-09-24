# kNN-Random-Forests-and-SVM

Classification techniques using kNN, Random Forests and SVM

## kNN

In this project we deal with the classification of breast tumour samples as ‘benign’ or ‘malignant’ based on 30 features. The column ‘DIAGNOSIS’ corresponds to the tumour classification where ‘B’ stands for ‘benign’ and ‘M’ for ‘malignant’. The other 30 columns correspond to the features.

First we train a k-Nearest Neighbour (kNN) classifier on the data set (tumour_samples.csv). We have used a grid search with 5-fold cross-validation to find an optimal value of the hyper-parameter k. Then we fix the optimal k and retrain the model on the entire data set tumour_samples.csv. We use accuracy to compare the performance of our optimised classifier on the data set tumour_samples.csv to the performance on the test data set tumour_test.csv.

## Random Forest