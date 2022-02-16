# Neural_Network_Charity_Analysis

## Overview
For this weeks project, we are tasked to use deep-learning neural networks with the TensorFlow platform in Python. We analyze and classify the success of charitable donations. Our data source is a csv file with data pertaining to charitable donations.
Our objectives are to

- Preprocess the data for the neural network model,
- Compile, train and evaluate the model,
- Optimize the model.

## Results

### Data Preprocessing 

 - The columns "EIN" and "Name" were not considered features, and therfore removed 
 - ![Screenshot (103)](https://user-images.githubusercontent.com/87949792/154371285-262d2ba0-d85b-44ab-92e2-a7f042d0b9dd.png)

- The column "IS_SUCCESSFUL" was the target variable
- ![Screenshot (104)](https://user-images.githubusercontent.com/87949792/154371531-1603ee23-fc88-456f-a6ea-793dfa5bb869.png)

- The columns 'APPLICATION_TYPE','AFFILIATION','CLASSIFICATION','USE_CASE','ORGANIZATION','INCOME_AMT', and'SPECIAL_CONSIDERATIONS' were features of the model 
- ![Screenshot (105)](https://user-images.githubusercontent.com/87949792/154372066-e544f21b-daa6-411d-8650-529944f83a44.png)


### Compiling, Training and Evaluating the Model

- This model has two hidden layers. Hidden layer 1 has 80 neurons, and hidden layer 2 has 30. The hidden layers used the ReLu activation functions and the output used the Sigmoid activation function. 
- ![Screenshot (106)](https://user-images.githubusercontent.com/87949792/154372565-4a7728ac-e7f2-4c6e-b58c-447305952ba4.png)

- The Model accuracy was 58%, which was not satisfactory
- ![Screenshot (107)](https://user-images.githubusercontent.com/87949792/154372860-149a4b86-ddb8-4b3b-a3b6-66273cb65e5e.png)

- Three attempts were made to increase the accuracy: we removed features from the model, we increaded the neurons and added 1 hidden layer, and lastly we changed the output activation function from Sigmoid to tanh. Unfortunately, none of these changes were able to bring the accuracy to above 75%.

## Conclusion

Unfortunately, none of our attempts with the deep learning neural network models got us to an accuracy of above 75%. This analyst reccomends using the supervised machine learning model Random Forest to see if that model can yeild a higher accuracy. 


