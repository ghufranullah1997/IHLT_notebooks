# Exercise 5:
We can trick our MLP model into learning task-specific feature importance by having it behave like a simple linear classifier, which learns a single real number for every feature (every word in our case), where the higher this number, the more strongly associated the feature is with one of the classes, and the lower this number, the more strongly associated the feature is with the other of the classes. The classifier then simply sums the weights of the individual features (i.e. there is no non-linearity in the hidden layer).

If this works, we should be able to sort the features (here: words) by this weight and get the "positive" words at one end, and "negative" words at the other end of this ordering.

Your task is to try this on the IMDB data and print the first few tens of words from both ends of this ordering. Did it work?

Hint: You can work from the IMDB classifier notebook, and really only need to implement minimal changes. To achieve such a linear classification based on a single weight for each feature (here: word), you will need to modify the size of the embedding matrix appropriately, and do a small change in the model's computation (forward method) to get rid of the nonlinearity.

Spoiler: This does work and if you did the exercise right, you should see a very clear pattern.
