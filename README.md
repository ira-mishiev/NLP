# NLP project

Abstract 

The new year 2022 has come with a tragic event in Europe; Russia has invaded Ukraine. This recent crisis may affect the lives of people of all west counties; therefore, not surprisingly, the conflict is broadly discussed throughout the world. Twitter is one of the most popular social media in English-speaking counties. Since the war between Ukraine and Russia started, the number of tweets has reached millions of tweets per day. For my project, I used tweets collected from just one day in the first week of invasion 02/27/2022. My purpose is to discover what underlying topic people are discussing and their sentiments about some events, counties, and people involved in this war.
Design
Due to the technologies, the information we receive online is highly customized. In other words, we are more likely to see information that we would have liked potentially and wanted to see. Therefore is easy to appear in a bubble of news and thoughts that are close to ours. NLP techniques can solve this pattern, helping to analyze data from people around the globe evenly. 

Data
I will use data from Kaggle that consists of 227 450 tweets of the one day of the war.
https://www.kaggle.com/code/alifiyabatterywala/ukraine-vs-russian-topic-modeling/data

Algorithms
Text Preprocessing: removed punctuation, links, hashtags, nicknames, and digits. Used WordNetLemmatizer, NLTK, SpaCy.
Topic Modeling: CountVectorizer, TF IDFVectorizer; for my data, better results showed TF IDFVectorizer. Then, I tried different topic modeling techniques like LSA, NMF, and LDA. After tuning hyperparameters like min/max doc frequency (max_df=0.8, min_df=0.01), number of topic = 5, I received the most interpretable results with NMF.
Sentiment: retrieved the most popular adjectives for some frequently appeared names from a corpus and used word2vec as another approach. 
  
Tools
For Topic modelling - Gensin,Sklearn
For sentiment analysis - SpaCy, word2vec
For text preprocessing NLTK
For visualization pyLDAvis, Matplotlib

Communication
The output of this project is showcased in the presentation

