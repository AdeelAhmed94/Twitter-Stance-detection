# Twitter-Stance-detection

Stance Detection of a tweet author against a given topic using transfer learning and fine tuned a pre-trained large BERT model

## INTRODUCTION
Social media platform like Facebook, discussion forums and especially Twitter have been widely used by people to express their opinion towards certain topics. Stance is the attitude the author has towards the topic which can be a person, government, organization or event. Tweet Stance Classification is the task of classify tweets posted on social media whether the tweets are in the favour, against or neutral for the given target which can be a person, a government, a company or anything. This classification task is different from sentiment analysis where we try to determine whether the text is positive, negative or neutral based up on the choice of the language used which can be either positive or negative. A tweet who is in favor of one target can be expressing stance against another target. For example, 
</br>*Target: Hillary Clinton*
</br>*My vote is for Hillary Clinton. I can’t trust a businessman @HillaryClinton*
</br>This tweet target is Hillary Clinton, and the tweet is in her favor, but this tweet is against the target Donald Trump
Recurrent Neural network and LSTM have proven well to work wells for language task because these networks can capture the sequential information from the text unlike traditional Neural Network. Training these networks from scratch requires a large amount of data for these models to converge and can be hardware dependent. Also, most of the work related to stance detection in tweets uses traditional deep learning approach. Here, we use start of the art language model BERT. By using transfer learning, we fine-tuned a pre-trained BERT model for our stance classification task. It is a bidirectional model and uses transformer which used to learn contextual meaning between words. Unlike directional models, it reads the entire sequence of words at once. We freezed the bert model and our own custom layers were attached to the bottom and then model was trained for detecting stance in a tweet for a given target.


## References

Saif Mohammad, Svetlana Kiritchenko, Parinaz Sobhani, Xiao-Dan Zhu, and Colin Cherry.A dataset for detecting stance in tweets. InLREC, pages 3945–3952, 2016a.
