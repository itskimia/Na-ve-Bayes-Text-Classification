# Naive-Bayes-Text-Classification

In this project, I implemented a Naïve Bayes classifier for classifying book reviews as positive or
negative. The dataset is a collection of Amazon user reviews about a book which is added as "reviews_train.csv". This project was done as my homework for the Data Mining course under supervision of Dr. Ehsan Nazerfard.

1) Preparing the data: I had to convert each review’s text to a bag of words
representation. So, the first task was to go through all reviews and construct a vocabulary
of all unique words. In this step I ignored all the stop words given in the ‘sw.txt’
file. The words must be extracted by splitting text off the whitespace characters and it is
recommended to convert all letters to lowercase. The next step is to get counts of each
individual word for positive and negative classes separately to get P(word|class).

2) Classification: In this step I needed to go through all the negative and positive samples
in the test set (added as "reviews_test.csv") and classify each one according to the
parameters learned earlier. The classification is done by comparing the log
posterior (P(X|Y)P(Y) for both classes.

3) Laplace Smoothing: An issue with Naïve Bayes classifier is that if a test sample contains a
word which is not present in the dictionary, P(word|class) equals to zero. To mitigate this
issue, one solution is to employ Laplace Smoothing (it has a parameter α). I then Enhanced my
classifier by employing Laplace Smoothing.
