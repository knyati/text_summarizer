# Text Summarizer

Hello there!!
This file refers to a text summarizer that I have coded using Keras framework using python on google colab. 

# Introduction

Text summarizer is simply a software that takes a large text corpus and gives a summary of the corpus.

It can be of two types
1) Abstractive: In this type of text summarizer a text corpus is given and a particular meaning or related sentences are taken as an output from the model.
These sentences/outputs need not be from the corpus itself.

2) Extractive:  In this type of text summarizer a text corpus is given and a particular set of sentences from the corpus itself are taken as output.

In this repository, I have made an abstractive summarizer.

## Frameworks and Libraries used

Here I am using python with inbuilt libraries like
1) Keras for Deep learning framework. 
2) BeautifulSoup and nltk for pre-processing.
3) Pandas and numpy for reading the data an data manipulation.
4) Matplotlib for plotting purpose.

## Dataset
 I have used Amazon fine food reviews dataset for training and validation set.
You can download it from here
[https://www.kaggle.com/snap/amazon-fine-food-reviews](https://www.kaggle.com/snap/amazon-fine-food-reviews)

## Model Description

I have used deep learning techniques for the implementation of the model.
Here we have used seq2seq encoder-decoder architecture.

For the encoder, there are 3 LSTM layers used and for the decoder, there is 1 LSTM layer used.

The outputs and the cell states of the last part of the encoder are passed to an attention layer from which the attention states are passed to the decoder which is to used to predict the outputs of the decoder which is also a sequence.

Please follow the .ipynb notebook for further proceedings.
