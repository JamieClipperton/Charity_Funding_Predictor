# Charity_Funding_Predictor
Deep Learning Homework: Charity Funding Predictor purpose/goal is to predict if the Alphabet Soup–funded organization will be successful.

### Preprocess the data

The target variable for the model will be "IS_SUCCESSFUL". This column has values of 1 and 0 which helps us determine if the charity fund is successful (1) or not successful(0).  After columns "EIN" and "Name" are dropped, the remaining columns are features for the model. 

### Compile, Train, and Evaluate the Model

Use TensorFlow to design a neural network, or deep learning model, to create a binary classification model that can predict if the organization will be successful based on the features in the dataset. Compile, train, and evaluate the binary classification model to calculate the model’s loss and accuracy.

**First Attempt** : Used neural network model with 2 hidden layers applied. First hidden layer with 9 nodes and second hidden layer with 25 nodes, using 100 epochs.
First Attempt resulted in a Loss of 0.5546 and Accuracy of 0.7240 (72%), does not hit target accuracy of 75%.

![image](https://user-images.githubusercontent.com/101610081/187514974-ab50b86c-0dde-4e85-b57a-1411e4aa8f13.png)

**Second Attempt** : Used neural network model with 3 hidden layers this attempt. First hidden layer with 80 nodes, second hidden layer with 60 nodes, and third hidden layer with 40 nodes. Used 100 epochs. 
Second Attempt resulted in a Loss of 0.587 and Accuracy of 0.7257 (73%), does not hit target accuracy of 75% but a little closer then first attempt. 

![image](https://user-images.githubusercontent.com/101610081/187515143-5d86d9bf-84bc-48bc-942b-4ba6060fbf3f.png)

**Third Attempt** : Used neural network model with 4 hidden layers this attempt. First hidden layer with 150 nodes, second hidden layer with 75 nodes, third hidden layer with 50, and fourther hidden layer with 25 
nodes. Used 100 epochs. 
Third Attempt resulted in a Loss of 0.5774 and Accuracy of 0.7254 (73%), 3 layers was closer then adding a 4th layer to the 75% target accuracy rate. 

![image](https://user-images.githubusercontent.com/101610081/187515328-63ef4729-468e-4848-a287-91beb3581d39.png)

**Fourth Attempt** : Went back to using neural network with only 3 hidden layers this attempt. First hidden layer with 50 nodes, second hidden layer with 30 nodes, and third hidden layer with 10 nodes, using 100 
epochs. 
Fourth Attempt resulted in a Loss of 0.5695 and Accuracy of 0.7263 (73%), did not hit the 75% target accuracy rate but fourth attempt came the closest out of all attempts. 

![image](https://user-images.githubusercontent.com/101610081/187515481-c84a3449-96d0-4e1e-a4aa-8d134f417e72.png)

I was not able to achieve the 75% target. I increased number of hidden layers on each attempt, and changed the number of nodes.

### Summary :

The results of each of my attempts did not reach the target accuracy rate of 75%. Increasing the number of layers did not improve accuracy as third attempt with four hidden layers returned a decreased 
accuracy rate compared to results from attempts two and four with three hidden layers. My recommendation would be to apply some feature reduction techniques to reduce the number of features applied, and 
adjusting the hyperparameters to get closer to the 75% desired accuracy rate.  


