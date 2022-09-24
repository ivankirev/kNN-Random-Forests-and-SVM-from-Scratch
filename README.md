# kNN-Random-Forests-and-SVM-from-Scratch

Classification by implementing kNN, Random Forests and SVM using only NumPy

## kNN

In this project we deal with the classification of breast tumour samples as ‘benign’ or ‘malignant’ based on 30 features. The column ‘DIAGNOSIS’ corresponds to the tumour classification where ‘B’ stands for ‘benign’ and ‘M’ for ‘malignant’. The other 30 columns correspond to the features.

First we train a k-Nearest Neighbour (kNN) classifier on the data set (tumour_samples.csv). We have used a grid search with 5-fold cross-validation to find an optimal value of the hyper-parameter k. Then we fix the optimal k and retrain the model on the entire data set tumour_samples.csv. We use accuracy to compare the performance of our optimised classifier on the data set tumour_samples.csv to the performance on the test data set tumour_test.csv.

## Random Forest

We train a random forest classifier on the data set tumour_samples.csv employing cross-entropy as our information criterion for the splits in the decision trees. We use 5-fold cross-validation subsets to explore and optimise over suitable ranges the following hyper-parameters:

1. number of decision trees

2. depth of trees.

We use accuracy as the measure of performance for this hyper-parameter optimisation.

We compare the performance of your optimal random forest classifier on the data set tumour_samples.csv to the performance on the test data tumour_test.csv using different measures computed from the confusion matrix, in particular commenting on accuracy, recall and F1-score.

## SVM

We train a soft margin linear SVM classifier on the data set tumour_samples.csv using 5-fold cross-validation subsets to optimise the hardness hyper-parameter that regulates the boundary violation penalty. We use accuracy as a measure of performance for this
hyper-parameter optimisation. We then display the accuracy of the SVM classifiers as the hardness hyper-parameter is varied, and discuss the limits of low hardness and high hardness.

We then evaluate the performance of the SVM classifiers obtained as the hardness hyper-parameter is varied by applying each of them to the test data tumour_test.csv. We represent our results using a receiver operating characteristic (ROC) curve. We use the ROC curve to discuss our choice of the optimal hardness hyper-parameter obtained above.

We then repeat this for the balanced data set tumour_samples_bal.csv. Using ROC curves (or other measures), we compare and discuss the performance of SVM classifiers learnt from the (unbalanced) data set tumour_samples.csv versus SVM classifiers learnt from the balanced data set tumour_samples_bal.csv.
