SENMETER
sentimental analysis

analyss the users sentiment based of social media posts

aim is to read texts from twitter and facebook files and use linguistic markers present in them to analyse mood. the mood analysed over the last 10 posts (or over time, if it is a frequent user) is the current mood. This shall also measure post interaction, i.e. if a user has been engaging with posts tagged as "sad" more recently the current mood will be hinting towrds sad.

current mood = [0,1,2,3,4] on a 5 point scale...0 being lowest.

The project aims at creating a ai system that analyses social media posts (Currently it imports tweets(texts) as csv and uses linguistic markers in them to judge the sentiment/mood of the user)(for eg a tweet "aw shucks, what a bad flight" will be marked in negative sentiment, (because of the word bad) Similarly for other emotions

I need it to scan the tags for pictures.. some pictures on the Internet can be found under certain tags.. I need it to look it up on the web, identify it's tag and classify it as sad/happy etc.. This will create 2 lists

A daily list
A weekly list
After 3-4 entries in the daily list.. It'll match the frequency of the entries [sad, sad, happy, sad, confused] This will be returned as 'sad' Then form the recommendation list(which can be modified according to user) it'll recommend some activities for a sad mood.

based of this the programme will have recommended activities. the programme will have a default set of recommended activities but it can be modified by th user according to their needs. the idea is to make it into an appliaction that sends the recommended activities as notifications.

I've used python to analyze tweets, the code in the above folder...

For the code to work you need to have a twitter.csv folder from where it'll analyse the tweets. IDE for pyhon,

libraries are:

import pandas as pd

import matplotlib.pyplot as plt

from tensorflow.keras.preprocessing.text import Tokenizer

from tensorflow.keras.preprocessing.sequence import pad_sequences

from tensorflow.keras.models import Sequential

from tensorflow.keras.layers import LSTM,Dense, Dropout, SpatialDropout1D

from tensorflow.keras.layers import Embedding

import time

import pandas as pd

import numpy as np

import matplotlib.pyplot as plt

import nltk

import io

import unicodedata

import numpy as np

import re

import string

from numpy import linalg

from nltk.sentiment.vader import SentimentIntensityAnalyzer

from nltk.tokenize import sent_tokenize, word_tokenize

from nltk.tokenize import PunktSentenceTokenizer

from nltk.tokenize import PunktSentenceTokenizer

from nltk.corpus import webtext

from nltk.stem.porter import PorterStemmer

from nltk.stem.wordnet import WordNetLemmatizer

df = pd.read_csv("./Tweets.csv")

WHATS NEEDED:

analyse pictures (by using tags in them) (specifically for instagram)
allow the user to input their own activity.
provide a user interface for modifying their recommended activity.[You have full freedom over this be as vreative as possible]
analyse images from facebook
code to monitor interaction time
How to Contribute? see Contribution.md https://github.com/TheCleverIdiott/SENMETER/blob/main/Contribution.md
