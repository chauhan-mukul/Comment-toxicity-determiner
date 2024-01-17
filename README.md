# Comment Toxicity Determiner

This model classifys the comment into [insult,toxic,severe_toxic,identity_hate,threat,obscene] on the bases of severity of the comment.

# Overview

The Comment Toxicity Determiner is a sophisticated tool designed to assess and identify the level of toxicity within written comments across various digital platforms. In the evolving landscape of online
communication, the need for effective moderation and the promotion of healthy discourse has become increasingly crucial. This tool employs advanced natural language processing (NLP) algorithms to analyze
the content of comments and evaluate the presence of toxic language, hate speech, and inappropriate expressions.

# Methodology

1st.  The given  Corpus  will be used to find total unique words in the corpus.<br>
2nd. The total words in the vocabulary will be mapped to unique integers to get a word_Index.<br>
3rd .Each comment in the corpus will be encodede to its word to integer mapping.<br>
4th. The comments that have been encoded are not of same length and we need to pad them to have them as inputs for our model.<br>
5th. The encoded corpus is large so we need to create batches and train the corpus in batches so the memory is not full.<br>
6th. We created a generator function.<br>
7th. Now pass the generator funciton to model and train it for 10 epochs(epochs can be increased to improve the accuracy of the model.<br>


