# 24

Thanks, Mike. 

After we get these 79 features, how can we deal with them? 

We compared the relative importance between these features. 

It is clear to see that some features are much more importance than the other feature.

# 25

To prove that, let me take the accommodates, also called the capacity of the house, as an example. This is the box plot between accommodates with price. We can clearly see the upward trend in the plot.

# 26

How about the irrelevant feature?

# 27

This is the box plot between the number of listings of host with price. It has little relation with the price. So we can't see any clear trend in this plot. 

# 28

Then let's talk something about our model building part. 

Basically, we use the pipeline method to fit and tune our model. 

As we all know, their are 3 parts of the whole method. 

That is the input, the output and inside the pipeline. 

First, the input model.  From the very beginning, we have tried Linear Regression, Decision tree, Bagging, Gradient Boosting, and many other models. 

Then is the dataset.  We split data into two groups, 80% for the train and the rest 20% is for the test.

Inside the pipeline, we tune our models. We use Grid Search and Cross Validation to tune our hyper-parameters of our model.

Finally, the output part. We can get the scores and the visuals to help us do further analysis.

Then let's us welcome Brian back to the stage!

