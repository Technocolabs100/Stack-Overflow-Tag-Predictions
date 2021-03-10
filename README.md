# Stackoverflow Tag Prediction

## Business Problem
Stack Overflow is the largest, most trusted online community for developers to learn, share their programming knowledge, and build their careers.<br>
Stack Overflow is something which every programmer use one way or another. Each month, over 50 million developers come to Stack Overflow to learn, share their knowledge, and build their careers. It features questions and answers on a wide range of topics in computer programming. The website serves as a platform for users to ask and answer questions, and, through membership and active participation, to vote questions and answers up or down and edit questions and answers in a fashion similar to a wiki or Digg. As of April 2014 Stack Overflow has over 4,000,000 registered users, and it exceeded 10,000,000 questions in late August 2015. Based on the type of tags assigned to questions, the top eight most discussed topics on the site are: Java, JavaScript, C#, PHP, Android, jQuery, Python and HTML.

## Problem Statemtent
Suggest the tags based on the content that was there in the question posted on Stackoverflow.

## Data Source
Source: https://www.kaggle.com/c/facebook-recruiting-iii-keyword-extraction/

## Real World / Business Objectives and Constraints
Predict as many tags as possible with high precision and recall.
Incorrect tags could impact customer experience on StackOverflow.
No strict latency constraints.

## Data Overview
Train.csv contains 4 columns: Id,Title,Body,Tags.<br>
Test.csv contains the same columns but without the Tags, which you are to predict.<br>
Size of Train.csv - 6.75GB<br>
Number of rows in Train.csv = 6034195<br>
The questions are randomized and contains a mix of verbose text sites as well as sites related to math and programming. The number of questions from each site may vary, and no filtering has been performed on the questions (such as closed questions).

## Key Performance Index
__Micro-Averaged F1-Score (Mean F Score):__ The F1 score can be interpreted as a weighted average of the precision and recall, where an F1 score reaches its best value at 1 and worst score at 0. The relative contribution of precision and recall to the F1 score are equal. The formula for the F1 score is:<br>

F1 = 2 (precision recall) / (precision + recall)<br>

In the multi-class and multi-label case, this is the weighted average of the F1 score of each class. <br>

__'Micro f1 score':__
Calculate metrics globally by counting the total true positives, false negatives and false positives. This is a better metric when we have class imbalance.<br>

__'Macro f1 score':__ 
Calculate metrics for each label, and find their unweighted mean. This does not take label imbalance into account.<br>

https://www.kaggle.com/wiki/MeanFScore<br>
http://scikit-learn.org/stable/modules/generated/sklearn.metrics.f1_score.html


## Prerequisites
You need to have installed following softwares and libraries in your machine before running this project.

1. Python 3
2. Anaconda: It will install ipython notebook and most of the libraries which are needed like sklearn, pandas, seaborn, matplotlib, numpy, scipy.
3. Word Cloud: https://pypi.org/project/wordcloud/

## Author
- Yasin Shah
