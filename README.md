## Abstract
Naive Bayes is among one of the simple algorithms for classification based on Bayes Theorem. Naive Bayes model is easy to build and particularly useful for very large data sets. There are two parts to this algorithm: <br />

Naive<br />
Bayes<br />

The Naive Bayes classifier assumes that the presence of a feature in a class is unrelated to any other feature. Even if these features depend on each other or upon the existence of the other features, all of these properties independently contribute to the probability that a particular fruit is an apple or an orange or a banana and that is why it is known as "Naive" (uneffected). 

## Bayes Theorem 
We have a Deck of Cards to find out the “Probability of the Card we picked at random to be a King given that it is a Face Card“. First, we need to find out the probability
<br />

![](https://github.com/Pramodgopinathan/Naive-Bayes/blob/8be41914ab4713eb7c5056c65a4d5691e2cdab65/Face%20Card.jpg)


P(King) which is 4/52 as there are 4 Kings in a Deck of Cards. <br />
P(Face|King) is equal to 1 as all the Kings are face Cards. (Probability of Face given King) <br />
P(Face) is equal to 12/52 as there are 3 Face Cards in a Suit of 13 cards and there are 4 Suits in total. <br />

P(King) = 4/52 = 1/13 <br />
P(Face|King) = 1 <br />
P(Face) 12/52 = 3/13 <br />

P(King|Face) = P(Face|King) * P(King) / P (Face) <br />

1 * (1/13) / 3/13 = 1/3 <br />

Now, putting all the values in the Bayes Equation we get the result as 1/3


## Navie Bayes

Our Data, which comprises of the Day, Outlook, Humidity, Wind Conditions and the final column being Play, which we have to predict.

![](https://github.com/Pramodgopinathan/Naive-Bayes/blob/3c9559c69ed81c97b83916f389cf4f2167fc3b32/Dataset.png)

First, we will create a frequency table using each attribute of the dataset.

![](https://github.com/Pramodgopinathan/Naive-Bayes/blob/e34b3a56c4282761e783f2bf91c2b03f59fdf071/Frequency%20table.png)

For each frequency table, we will generate a likelihood table.

![](https://github.com/Pramodgopinathan/Naive-Bayes/blob/5986fd11d92c8ce8d2696382217cc85acdcd7522/likelihood.png)

Likelihood of ‘Yes’ given ‘Sunny‘ is:
P(c|x) = P(Yes|Sunny) = P(Sunny|Yes)* P(Yes) / P(Sunny) = (0.3 x 0.71) /0.36  = 0.591

 
<br />
Similarly Likelihood of ‘No’ given ‘Sunny‘ is:
P(c|x) = P(No|Sunny) = P(Sunny|No)* P(No) / P(Sunny) = (0.4 x 0.36) /0.36  = 0.40 <br />

Now, in the same way, we need to create the Likelihood Table for other attributes as well.

### Suppose we have a Day with the following values :
<br />
Outlook   =  Rain <br />
Humidity   =  High <br />
Wind  =  Weak <br />
Play =?
<br />
Likelihood of ‘Yes’ on that Day = P(Outlook = Rain|Yes)*P(Humidity= High|Yes)* P(Wind= Weak|Yes)*P(Yes)
<br /> 
<br /> 

Calculating likelihood for each attributes will gives playing or not

### Conclusion
Naive Bayes classifiers are a popular used for e-mail filtering. They typically use a bag of words features to identify spam e-mail, an approach commonly used in text classification. Naive Bayes classifiers work by correlating the use of tokens (typically words, or sometimes other things), with a spam and non-spam e-mails and then using Bayes theorem to calculate a probability that an email is or is not spam.

#### Benefits: <br />
It is simple and easy to implement
It handles both continuous and discrete data
It is fast and can be used to make real-time predictions
 <br />
#### Disadvantages: <br />
Naive Bayes assumes that all predictors (or features) are independent, rarely happening in real life. This limits the applicability of this algorithm in real-world use cases.

### Python Code

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/Pramodgopinathan/Naive-Bayes/blob/main/Naive_Bayes.ipynb]

