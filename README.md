# Prediction-of-reactions-to-the-posts-test-task

## Preprocessing

- replace all urls with "__URL__" token

- replace all user references with "__AT_USER__" token

- replace all emojis with equivalent words (e.g. ":)" with "cheer")

- removing numbers

## Feature extraction

Features fall into two categories - tf-idf features and emotion features.

Emotion features were obtained using combination of NRC-emotion-lexicon and WordNet datasets (for each word in NRC-emotion-lexicon synonyms of this word from WordNet was also considered). 

## Model training

Support vector classifier was trained on these features

## Accuracy

f1 score: 0.66

accuracy score: 0.8
