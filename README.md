Authors: Joshua Zwiebel and Teva Zanker

# Tweet-Sentiment-Extraction
A repository detailing work involved in the kaggle competition Tweet Sentiment Extraction



# Tweet-Sentiment-Extraction
A repository detailing work involved in the kaggle competition Tweet Sentiment Extraction



## Purpose and Overview

The purpose of this repository is twofold. Firstly it is to compete in the [Tweet Sentiment Extraction](https://www.kaggle.com/c/tweet-sentiment-extraction/overview) kaggle competition. Secondly, it is to document all the thought process and mistakes made while adhering to a data science workflow. You will find many cells that throw runtime errors. This is by design we wanted to keep the cells with errors and demonstrate how we fixed the problems as opposed to working backwards and leaving the reader the impression that everything worked on first attempt. We found there is a lot of value to be had in seeing where mistakes were made. 

# The Data

The data being processed was as follows (it can be found within the repository for further inspection). A single sample contains up to 4 data points
- The text of the tweet
- a sentiment of the tweet (i.e positive)
- a unique identifier for the tweet
- the keywords that exemplify the sentiment

They keyword and location of the tweet had the potential to be blank. The training data contained approx ~27000 samples and more detail into the composition of the data can be found within the exploration folder.

# Preprocessing
A couple of different strategies were taken during the preprocessing phase. Cleaning of the data was important. This step involved stripping punctuation and and suffixes from words. As the data came from tweets many of the words were mispelled. We employed pyspellchecker in order to spellcheck all of the tweets simultaneously. The computation was lengthy but completed after running overnight. We then had to employ feature engineering. We knew that because the selected text was taken right from the original tweet it would be a good idea to instead predict the indices of the words that would be usued for the selected text as opposed to predicting the words themselves


# Models


# Resources and Learning


# Results 

# Future Work and Concessions made


# How to use any of the Code
Install the requirements.txt and start running the notebooks! If you encounter any issues please post an issue or email me and jjzwiebe@uwaterloo.ca. Starting with the exploration folder is likely the best place to start.
