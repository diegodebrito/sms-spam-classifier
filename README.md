# SMS Spam Classifier


In this project, I use Machine Learning methods to classify SMS messages in spam or ham (i.e. legitimate messages). The dataset consists of 5574 English, real and non-encoded messages that are tagged as spam or ham.

The dataset comes from the original source: http://www.dt.fee.unicamp.br/~tiago/smsspamcollection/


### Results


The final pipeline configuration achieves a F1-score of 0.96 on previously unseen data (I use 80% of the data for training, 10% for validation and 10% for testing). Out of 558 messages on the test set, our final model only has 2 false positives (saying that something is spam when it is not) and 4 false negatives (saying that something is not spam when in fact it is). These numbers correspond to a precision rate of 97% and a recall rate of 95%.


### Models and Techniques


- Models: Logistic Regression, Random Forest Classifier, Bernoulli Naive Bayes and Multinomial Naive Bayes.
- Text processing: regular expressions, CountVectorizer and TF-IDF.
-  Feature Engineering (new features such as word count, punctuation count).
-  Undersampling.
