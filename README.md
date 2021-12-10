## Abstract
Naive Bayes is among one of the most simple and powerful algorithms for classification based on Bayes Theorem. Naive Bayes model is easy to build and particularly useful for very large data sets. There are two parts to this algorithm: <br />

Naive<br />
Bayes<br />

The Naive Bayes classifier assumes that the presence of a feature in a class is unrelated to any other feature. Even if these features depend on each other or upon the existence of the other features, all of these properties independently contribute to the probability that a particular fruit is an apple or an orange or a banana and that is why it is known as "Naive" (uneffected). 

## Bayes Theorem 
We have a Deck of Cards to find out the “Probability of the Card we picked at random to be a King given that it is a Face Card“. First, we need to find out the probability
<br />
P(King) which is 4/52 as there are 4 Kings in a Deck of Cards. <br />
P(Face|King) is equal to 1 as all the Kings are face Cards. <br />
P(Face) is equal to 12/52 as there are 3 Face Cards in a Suit of 13 cards and there are 4 Suits in total. <br />

P(King) = 4/52 = 1/13 <br />
P(Face|King) = 1 <br />
P(Face) 12/52 = 3/13 <br />

P(King|Face) = P(Face|King) * P(King) / P (Face) <br />

1 * (1/13) / 3/13 = 1/3 <br />

Now, putting all the values in the Bayes Equation we get the result as 1/3

