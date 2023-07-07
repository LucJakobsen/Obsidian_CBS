``from sklearn.model_selection import train_test_split``
A Scikit-learn model ([[Python Libraries]]) that will split the data into a training set and a data set. This separation is necessary because it allows us to determine how well our model can predict "new" data. 
- So we use some of the data to feed the model, and some to test how accurate it is

"New" data = data that the model has not seen before. 

If we train the model using a data set, then evaluate the model using the same data set, we would have no way to determine whether the model is good at fitting "new" data or only good at fitting the data it has already seen.

We can randomly or nonrandomly split the data.

We can also cross validate the training and test sets. This is called [[K-fold Cross Validation]].



### Arguments:
- ``test_size`` = defines what percentage of the split should go to the test set
- ``random_state`` =  