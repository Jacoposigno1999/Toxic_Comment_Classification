# Toxic Comment Classification

For this NLP project we have been assigned a [Dataset](https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge/data) containg a large number of Wikipedia comments which have been labeled by human raters for toxic behavior.  The types of toxicity are:
- toxic
- severe_toxic
- obscene
- threat
- insult
- identity_hate

## Goal of the project 
The goal of this project was to create a **multi-label classication model** which predicts the probability for each type of toxicity for a given comment.

## Our approaches

We decided to try to achieve this goal through the implementation of 2 different models:
- A "simple" RNN architecture, more preciselly a BLSTM (Bidirectional Long Short-Term Memory)
- A more advanced trasformer based architecture(BERT).

##Achieved results

![image](https://user-images.githubusercontent.com/109806659/210773695-7c5305af-554a-4be7-b623-809c7d443324.png)

As we can see, and as we expected, with the BERT model we achive much better result. In general we have higher precision, recall and f1-score for all the categories, but most importantly we can see how BERT successfully manages to predict even the less represented classes such as threat and identity hate, although it's still struggling with sever toxic.
