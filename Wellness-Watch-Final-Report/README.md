# Wellness-Watch

Machine learning models to perform sentiment analysis for mental health statuses.

Training and testing data can be found in `kaggle-sentiment-data.csv`.

## Baseline Model

The original model created by Muhammad Faizan, a researcher on Kaggle, can be found in `sentiment-analysis-for-mental-health-nlp.ipynb`.

This model utilizes logistic regression classification. However, this model was discovered to have data leakage into the test set due to data augmentation occuring before the data was split into train and test sets. A new baseline model was created to move data augmentation after the data is split into train and test sets in order to prevent data leakage into the test set. This model can be found in `baseline_sentiment-analysis-for-mental-health-nlp.ipynb`.

## Students' Models

### Logistic Regression (improved)

An improved model can be found in `logistic_regression.ipynb`.

This model improves upon the baseline model by removing data augmentation, changing hyperparameters, stratifying the status in train-test split, and making slight modifications to preprocessing.

### Random Forest

The model can be found in `random_forest.ipynb`.

### Naive Bayes Classifier

The model can be found in `naive_bayes_classifier.ipynb`.

### Gradient Boosting Machine

The model can be found in `gradient_boosting_machine.ipynb` which runs GridSearchCV to find the best parameters for the model.

The model found in `gradient_boosting_machine_best_params.ipynb` uses the parameters obtained from `gradient_boosting_machine.ipynb` to get the best accuracy for this model.

### Support Vector Machine

The model can be found in `support_vector_machine.ipynb` which runs GridSearchCV to find the best parameters for the model.

The model found in `support_vector_machines_best_params.ipynb` uses the parameters obtained from `support_vector_machine.ipynb` to get the best accuracy for this model.


## Member Contributions

Amy:
Before the midterm report, Amy was responsible for the initial testing of barebones machine learning models, researching Random Forest Classification, and writing the Proposed Extensions section of the paper. After the midterm report, Amy was responsible for implementing and analyzing the data augmentation preprocessing, Logistic Regression, and Random Forest models.


Kaylee:
Before the midterm report, Kaylee was responsible for researching and implementing preprocessing techniques and writing the introduction of the paper and the abstract. After the midterm report, Kaylee was responsible for implementing and analyzing lemmatization and the BERT model. Kaylee was responsible for writing the Abstract, Motivation, and Methodology sections of the poster.


Valli:
Before the midterm report, Valli was responsible for researching Logistic Regression Techniques and for writing the Baseline Solutions section of the paper. After the midterm report, Valli was responsible for implementing and analyzing SVM, Naive Bayes, and Gradient Boosting models. 


All members contributed to writing the Results and Analysis/Conclusion sections of the poster. All members contributed to acquiring data for the posters' graphs and Kaylee was responsible for creating them.
