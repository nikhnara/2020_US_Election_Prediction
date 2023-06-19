# 2020_US_Election_Prediction
To predict the 2020 US presidential election results using Sentiment Analysis on twitter historical data using roBERTa model


As we all know Twitter had played a key role in 2020 US Presidential election.
Twitter became one of the important platform for both democrats and republicans during the time of election to share their manifests and criticize their oppositions.
It had arranged many polls before and after the election day to know the public opinion.
How did Twitter use the public opinions or tweets to play a crucial role in elections? What type of model did it use to understand the pulse of voters?
Aim: 
To predict the 2020 US presidential election results using Sentiment Analysis on twitter historical data.

Objectives:
Sentiment analysis on the twitter dataset using Natural Language Processing (NLP). NLP helps machines process and understand the human language so that they can automatically perform repetitive tasks.
Sentiment analysis which is a NLP technique used to determine whether data is positive, negative or neutral.
Clustering and Mapping the sentiments to understand the spatial distribution of the voters sentiment



RoBERTa: RoBERTa was trained on a larger and more diverse corpus of text. This allows RoBERTa to learn more general and robust language representations that can be applied to a wider range of downstream NLP tasks.
High accuracy on complex texts, Pre-trained models available, High computational resources required ,Low interpretability
Text often used in social media are in informal language and contain lot of noise within them which makes it hard to understand the contextual meaning of the tweets.
RoBERTa uses masked language modelling which can be used to predict the sentiment of text on contextual bases.
“CardiffNLP/Twitter-RoBERTa-base-sentiment” is a pre-trained sentiment-analysis model that is pre-trained on social media text, including tweets.
Additionally it is fine tuned on sentiment analysis tasks, allowing to accurately classify the sentiment of tweet.
Based on the factors considered, we selected “CardiffNLP/Twitter-RoBERTa-base-sentiment” as our sentiment analysis model due to its high accuracy and availability of pre-trained models and predicting results based on contextual approach.
I have imported pipeline from the transformers and created a sentiment analysis pipeline to import the ‘Cardiffnlp/Twitter-RoBERTa-base-sentimen’t model and running the input text through the model to generate a sentiment prediction.
As our data size is very large and our model consumes more computational power we have chosen “Batch processing” approach to reduce the run time and load.
Now we have renamed the label_0 as negative, Label_1 as neutral, Label_2: Positive and assigned those values to new column “label” and respective scores to column “score”.
Now based on this label and scores we are going to visualize our data to interpret our results

<img width="543" alt="image" src="https://github.com/nikhnara/2020_US_Election_Prediction/assets/129335928/5df1c234-0ffb-4979-a1a8-8b2f6eae14e6">
<img width="548" alt="image" src="https://github.com/nikhnara/2020_US_Election_Prediction/assets/129335928/68806757-c1de-4cde-90fc-7a69a2f3fb82">
