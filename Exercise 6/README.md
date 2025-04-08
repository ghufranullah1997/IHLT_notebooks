# Exercise task 6: hyperparameters
Training the model depends on numerous hyperparameters. Among the most important once are the learning rate, batch size, naturally the model's parameters such as the length of the embeddings, and data parameters such as the maximum vocabulary size. It is good to gain some insights as regards to their possible effects on the results.

Try to adjust the various parameters and observe the results (for instance in terms of how quickly the training peaks and what the maximum observed performance is). Keep a little log in a new cell in the notebook at the very bottom, with your observations of what happens with different parameter values. 

At the minimum, try changing the learning rate (usually this is done in orders of magnitude, so 1e-1, 1e-2, 1e-3 ... etc.) You can also try to change the batch size, e.g. in powers of 2: 10, 20, 40, ... etc to see some effect. 
