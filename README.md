# Climate-pred-CCM
Repository for the final project of Cognitive Computational Modeling of Language and Web Interaction

## Proposal

Project proposal: Luuk Arts (s4396863) & Jordy Ripperda (s4381386) & Jesse Zwamborn (s4314182)

For our final project we propose to conduct a study where we predict climate and time aspects (e.g. weather, season, month, day) based on Twitter messages. This way we can investigate the effect seasonal features have on the sentiment expressed in tweets.

To do so, we found the sentiment140 dataset on Kaggle (https://www.kaggle.com/kazanova/sentiment140/data)  which contains 1.6 million tweets plus features as the polarity of the tweet (0 = negative, 2 = neutral, 4 = positive), the date of the tweet, the user, and the text itself.
 

The first study we found which could contribute to ours is [1], which sort of did the opposite of what we are planning to do. They used features such as geography, season, weather, and time (i.e. day-of-the-month/week) to predict the sentiment of tweets. The methods they use are decision trees. Although we don’t know the exact methods we will use in our study, we are thinking about more advanced machine learning techniques in order to make our predictions.

 

A possible technique we could use is the the one that is used in [2]. In their research they used a Bayesian approach to create a Twitter sentiment classifier, based on the author, location and the time of tweets.

 

[1] Hannak, A., Anderson, E., Barrett, L. F., Lehmann, S., Mislove, A., & Riedewald, M. (2012, June). Tweetin'in the Rain: Exploring Societal-Scale Effects of Weather on Mood. In ICWSM.

 

[2] Vosoughi, Soroush, Helen Zhou, and Deb Roy. "Enhanced twitter sentiment classification using contextual information." arXiv preprint arXiv:1605.05195 (2016).
