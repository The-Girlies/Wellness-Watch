# Wellness-Watch

Machine learning models to perform sentiment analysis for mental health statuses.

Training and testing data can be found in `kaggle-sentiment-data.csv`.

## Baseline Model

The original model created by Muhammad Faizan, a researcher on Kaggle, can be found in `sentiment-analysis-for-mental-health-nlp.ipynb`.

This model utilizes logistic regression classification. However, this model was discovered to have data leakage into the test set due to data augmentation occuring before the data was split into train and test sets. A new baseline model was created to move data augmentation after the data is split into train and test sets in order to prevent data leakage into the test set. This model can be found in `baseline_sentiment-analysis-for-mental-health-nlp.ipynb`.

## Students' Models

### Logistic Regression (improved)

An improved model can be found in `amy_logreg_sentiment-analysis-for-mental-health-nlp.ipynb`.

This model improves upon the baseline model by removing data augmentation, changing hyperparameters, stratifying the status in train-test split, and making slight modifications to preprocessing.

### Random Forest

The model can be found in `rf_sentiment-analysis-for-mental-health-nlp.ipynb`.
