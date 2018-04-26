# Climate-pred-CCM
Repository for the final project of Cognitive Computational Modeling of Language and Web Interaction

## Proposal

Project proposal: Luuk Arts (s4396863) & Jordy Ripperda (s4381386) & Jesse Zwamborn (s4314182)

For our final project we propose to conduct a study where we predict climate and time aspects (e.g. weather, season, month, day) based on Twitter messages. This way we can investigate the effect seasonal features have on the sentiment expressed in tweets.

### Dataset

To do so, we found a dataset that is a part of the Kaggle competition "Partly Sunny with a chance of Hashtags", a CrowdFlower competition (https://www.kaggle.com/c/crowdflower-weather-twitter). It consists of about 78.000 training tweets which are labeled as follows:

s = sentiment
w = when
k = kind

s1,"I can't tell"
s2,"Negative"
s3,"Neutral / author is just sharing information"
s4,"Positive"
s5,"Tweet not related to weather condition"  
w1,"current (same day) weather"
w2,"future (forecast)"
w3,"I can't tell"
w4,"past weather"
k1,"clouds"
k2,"cold"
k3,"dry"
k4,"hot"
k5,"humid"
k6,"hurricane"
k7,"I can't tell"
k8,"ice"
k9,"other"
k10,"rain"
k11,"snow"
k12,"storms"
k13,"sun"
k14,"tornado"
k15,"wind"

We plan to extend this dataset with a few variables (time/day/etc) by using the twitter API to gather more information about the tweets.

### Approach

Our plan is to build a text classifier that can predict these labels on the test set (42.000 tweets). Our initial plan is to use a dedicated tweet NLP (http://www.cs.cmu.edu/~ark/TweetNLP/) to analyze the tweets. For feature extraction we plan to use basic tf-idf, n-grams as a starting point.

Most competitors in the kaggle competition used a version of Ridge Regression to fit the data - we plan to also do this in Python, using the sklearn General Regression module (http://scikit-learn.org/stable/modules/linear_model.html#ridge-regression).


### Prior Research

The first study we found which could contribute to ours is [1], which sort of did the opposite of what we are planning to do. They used features such as geography, season, weather, and time (i.e. day-of-the-month/week) to predict the sentiment of tweets. The methods they use are decision trees. 

A possible technique we could use is the the one that is used in [2]. In their research they used a Bayesian approach to create a Twitter sentiment classifier, based on the author, location and the time of tweets.

 

[1] Hannak, A., Anderson, E., Barrett, L. F., Lehmann, S., Mislove, A., & Riedewald, M. (2012, June). Tweetin'in the Rain: Exploring Societal-Scale Effects of Weather on Mood. In ICWSM.

 

[2] Vosoughi, Soroush, Helen Zhou, and Deb Roy. "Enhanced twitter sentiment classification using contextual information." arXiv preprint arXiv:1605.05195 (2016).
