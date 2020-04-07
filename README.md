This repository contains the codes and Submission for SemEval 2019 Task 9 - SubTask A - Suggestion Mining from Online Reviews and Forums https://competitions.codalab.org/competitions/19955

## Details of the directory structure and file:

1. The data cleaning process is shown with comments in the Data_Pre_Processing.ipynb file
2. Three word representations are used for encoding the model- Fast Text, Word2Vec and Glove. For the three representations a sequence generator is made to produce the final sequences that will be the input to different models.
3. Differenet models (CNN,RNN,with/without Attention) are then tested on these sequence generators. And the results are summarised here.
4. CNN models with the BERT embeddings are also tested.  
5. ./Data directory contains the temporary data being saved and load by the different models. 
5. ./models directory contains the saved models for further use. 
6. We also tried improving the model further by more cleaning and handling the data imbalance as shown in the SequenceGeneratorFastTextSMOTE.ipynb file
 and tested in on CNN FastText with attention and CNN FastText without attention, but there was no improvment so we avoided handling data imbalance.

## Summary:

| Model Type    | Word Embedding| Attention      | Testing Accuracy      | F1 Score      |
| :---:         | :-:           | :-:            |:-:                    |:-:            |
| LSTM          | Word2Vec      | No             |   77.20%              |75.14%         |
| LSTM          | Word2Vec      | Yes            |   76.01%              |73.21%         |
| LSTM          | FastText      | No             |   77.87%              |77.76%         |
| LSTM          | FastText      | Yes            |   77.86%              |75.84%         |
| LSTM          | Glove         | No             |   78.21%              |76.16%         |
| LSTM          | Glove         | Yes            |   77.20%              |74.86%         |
| CNN           | Word2Vec      | No             |   80.07%              |79.08%         |
| CNN           | Word2Vec      | Yes            |   82.09%              |82.21%         |
| CNN           | FastText      | No             |   80.74%              |79.79%         |
| CNN           |FastText(SMOTE)| Yes            |   77.53%              |77.42%         |
| CNN           | FastText      | Yes            |   80.24%              |79.79%         |
| BERT          | -             | No             |   80.91%              |80.62%         |
| BERT          | -             | Yes            |   82.60%              |82.64%         |
