# SillyBasic - NLP In Python From Scratch

## What Is Machine Learning

At the very basic level, machine learning is statistics and mathematics. One of the most basic algorithm in machine learning is as shown below - linear regression.

![Linear Regression][linear_reqression]

As we see here, we have plotted some points along X-Y axis. We have fitted a line along these points. Now, say, we want to predict a new value, how do we do that? We do so by finding a point along X axis, getting that point in line, and then finding the corresponding Y value.

This is an example of prediction. What do we do in classification, another common task done by machine learning? Let's look at K nearest neighbors, another common and easy to understand algorithm in machine learning.

![K Nearest Neighbors][k_n_n]

We see we have from some clusters/groups based on nearest points the points have. How do we find the group/classification of a new point? By simply taking the nearest points and finding the group they belong to.

## The Problem - Machine Learning Only Works With Numbers

Since ML is just maths and statistics, it ultimately boils down to numbers. Now that's a problem with categorical data and text. So we use various methods to overcome that.

## Machine Learning With NLP - Bag Of Words

In Bag of Words, we take a text like below:

```
It was the best of times,
it was the worst of times,
it was the age of wisdom,
it was the age of foolishness
```

and convert that to numerical representation like below

```
it: 4
was: 4
the: 4
best: 1
worst: 1
age: 2
of: 4
times: 2
wisdom: 1
foolishness: 1
```

Now, we can predict if other texts belong to the same category or not, depending on the number of words match that of above or not.

## The Problem - The Larger The Text Is - The More The Words Will Have Scores

To overcome that, we use various methods:

* we ignore case
* we ignore punctuation
* we ignore common words (a, the etc) called stop words
* we fix misspelled words
* we reduce words to their stem

However, still it doesn't fix our main problem. To fix that, we use something called TF-IDF

## TF-IDF

We take the frequency of the words and score it. Then we see how rare it is across documents. The more rare it is, the higher it is scored.

## Naive Bayes Classifier

![Naive Bayes][naive_bayes]

[linear_reqression]: /assets/01.jpg "Linear Regression"
[k_n_n]: /assets/02.jpg "K Nearest Neighbors"
[naive_bayes]: /assets/03.png "Naive Bayes"