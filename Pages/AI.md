- ### *Steps*
	-
	- ### Take Input
	- ### Determine mood
		- [AI Mood Level detection ](https://www.geeksforgeeks.org/project-idea-ai-therapist/)
		-
		- ``import numpy as np
		  import pandas as pd
		  from pandas import Series, DataFrame
		  import matplotlib.pyplot as plt
		  import seaborn as sns
		  import string
		  from nltk.corpus import stopwords
		  
		  from sklearn.pipeline import Pipeline 
		  from sklearn.naive_bayes import MultinomialNB
		  from sklearn.feature_extraction.text import CountVectorizer as cv
		  from sklearn.feature_extraction.text import TfidfTransformer
		  #data is our input dataset containing user input lines and it has a column of emotional class. 
		  #The code will not work in IDE as no dataset has been provided
		  
		  
		  #function to remove punctuations and stopwords
		  def function_preprocess (mess):
		    nopunc = []
		    for char in mess :
		        if char not in string.punctuation:
		            nopunc.append(char)
		    nopunc=''.join(nopunc)
		    clean = []
		    for word in nopunc.split():
		        word = word.lower()
		        if word not in stopwords.words('english'):
		            clean.append(word)
		    return clean ``
		- #building our NLP model using naive bayes as classifier
		  pipeline = Pipeline([('bow', cv(analyzer=function_preprocess)),
		                    ('tfidf', TfidfTransformer()),
		                    ('classifier', MultinomialNB()),
		                    ])
		  pipeline.fit(data, emotional_class)``
		-
		- #### *if no flagged mood anwser any user questions*
		-
-