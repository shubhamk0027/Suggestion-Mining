This repository contains the codes and Submission for SemEval 2019 Task 9 - SubTask A - Suggestion Mining from Online Reviews and Forums [https://competitions.codalab.org/competitions/19955]

## Details of the directory structure and file:

Two models have been tried on first using the decison tree and other using the rnn classifier.

First model is build using the XGBoost decision tree, with 50% accuracy.
1. Data Cleaning Process is shown in the DataCleaning.ipynb
2. And the word2Vector representation of the cleaned data is in the ToWordVecEmbedding.ipynb file
3. And the XGBoost classifier is in the XgBoostClassifier.ipynb file.

All the process regarding the second model the RNN classifier with 87% accuracy is shown in the RnnClassifier.ipynb file.

All the models saved are in the ./model directory 

All the training data, testing data, data after cleaning, and the submissions are in the ./data structure


## Submission
Our final submission (./data/submission.csv) is made using the RNN classifer with 87% accuray on the Subtask A trial testing data.
RnnClassifier.ipynb contains all the final code along with detailed comments.
