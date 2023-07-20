# LHL Final Project: NLP Analysis of ADHD Reddit
An NLP sentiment analysis and topic modelling of an all-female ADHD Reddit board, using VADER, Word2Vec, lemmatization, and LDA. 
The aim of this project is to see how these NLP techniques function on a messgae board rather than other forms of social media that either have explicit limits in the length of texts (Twitter) or that have social conventions that make posts relatively short (Instagram) or private (Facebook). The analysis provides an overview of what topics matter to the target audience and whether the tone or valence of posts affects how Redditors react to the post through upvotes or downvotes.

Sentiment Analysis
Unlike reviews, where the writer is expected to indicate how much they like or do not like something and might attach a metric like three stars or a rating of 7 out of 10, message boards are open in subject matter and often will not contain any endorsement. So an unsupervised learning method was needed, as there is no overt metric for labelling a post as positive, negative, or neutral. VADER (Valence Aware Dictionary sEntiment Reasoner) allows for supervised or unsupervised learningin both classification or regression problems. Its Sentiment Intensity Analyzer can perform such a task, as it has a pre-trained dictionary of words rated for their emotional content and intensity. The SIA creates four scores for each text body: the percentage that each post if positive, negative, or neutral, summing to 100%, and a compound score synthesizing the other three. The goal was to see if any of these ratings correlated with the upvote score from Redditors reacting to a post.

Topic Modelling
Gensim's Latent Dirichlet Allocation (LDA)

# Data Preparation
The dataset is from Kaggle: https://www.kaggle.com/datasets/jerseyneo/reddit-adhd-dataset
This dataset has the time and date, the "score" or the balance of upvotes (+1) and downvotes(-1), and the content of months of messgaes posted, more than 203,000.

#
