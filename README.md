Tweet Sentiment Classification
===
In this project, I implemented a sentiment classification algorithm using single hidden layer neural network that classifies the sentiment of a tweet/sentence giving the dominant emotion(s) e.g. anger,sadness,fear or joy in the text.

<image>  </image>

How It Works
-------
In this project i read a large Tweet dataset and clean each tweet then use Stemming and using bag of words model, feed each tweet to single layer neural network for classification. Link for dataset is given below:
        http://saifmohammad.com/WebPages/EmotionIntensity-SharedTask.html

This link has 4 kinds of dataset: one for anger, one for fear, one for joy and one for sadness for training set and 4 files for test set. Each of these datasets have the following format:
All sentences start with a 

[number, tweet_sentence, label [fear,anger,joy,sadness], intensity_of_emotion].

The intensity of emotion varies from 0 to 1 where 1 expresses high intensity of anger, fear, joy or sadness. It is seen that only tweets with threshold higher than 0.5 or 0.6 “ACTUALLY” express the sentiment strongly. I am using this threshold which leaves us with the following:

Anger_training_set: emotion intensity threshold 0.5 411 lines

Fear_training_set: emotion intensity threshold 0.6 347 lines 

Joy_training_set: emotion intensity threshold 0.5 405 lines

Sadness_training_set: emotion intensity threshold 0.5 384 lines

In total I have 1547 lines in training data and total 4895 unique words that includes emoticons

Acknowledgement
----------------
I would like to give credit to this article "https://machinelearnings.co/text-classification-using-neural-networks-f5cd7b8765c6" for useful insights that helped me learn about this project and while the article is based on text classification using 2 hidden layer neural network with sigmoid activation function, I did Tweet sentiment classification using single hidden layer neural network with Relu activation function.
