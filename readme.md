


Initially I included all columns excluding the y column ("koi_disposition") in X.
using train_test_split from the sklearn.model_selection, the data is split between testing and training, using a random state of 1.
The feature check was run after the tests were completed, 
all columns
    SVC linear
    Training Data Score: 0.8584934431229033
    Testing Data Score: 0.8522415370539799
    GridSearchCV
    {'C': 10, 'gamma': 0.0001}
        0.8732845379688929
    RandomForest: 
    0.8902104300091491
results after removing columns with importance less than .01 using RandomForestClassifier
    SVC linear
    Training Data Score: 0.8571210734980177
    Testing Data Score: 0.8554437328453797
    GridSearchCV
    {'C': 10, 'gamma': 0.0001}
    0.8752668496492834
    RandomForest: 
    0.8902104300091491
scaling and spliting the data was the basic code used in all of our activities
I managed to get the best score using RandomForest. 

