This repository contains the codes and Submission for SemEval 2019 Task 9 - SubTask A - Suggestion Mining from Online Reviews and Forums https://competitions.codalab.org/competitions/19955

## Details of the directory structure and file:

Various models have been tried on first using the decison tree and then using the rnn and cnn classifier.

First model is build using the XGBoost decision tree, with 99% accuracy!
1. Data Cleaning Process is shown in the XgBoost1-DataCleaning.ipynb
2. And the word2Vector representation of the cleaned data is in the XgBoost2-WordVecEmbedding.ipynb
3. And the XGBoost classifier is in the XgBoost3-Classifier.ipynb file.

All the models saved are in the ./model directory 
All the training data, testing data, data after cleaning, and temporary data used are in the ./Data Directory

## Summary:

| Model Type    | Word Vector   | Attention      | Testing Accuracy      | F1 Score      |
| :---:         | :-:           | :-:            |:-:                    |:-:            |
| LSTM          | Word2Vec      | No             |   82.94%              |76.57%         |
| LSTM          | Word2Vec      | Yes            |   85.30%              |82.63%         |
| LSTM          | FastText      | No             |   77.70%              |76.70%         |
| LSTM          | FastText      | Yes            |   79.22%              |79.40%         |
| CNN           | Word2Vec      | No             |   92.91%              |91.73%         |
| CNN           | Word2Vec      | Yes            |   93.75%              |92.59%         |
| CNN           | FastText      | No             |   78.21%              |76.92%         |
| CNN           | FastText      | Yes            |   81.08%              |80.89%         |
| XGBoost       | Word2Vec      | No             |   99.83%              |99.83%         |
