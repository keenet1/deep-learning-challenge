# Overview:

The purpose of this activity was to create a neural network model for the nonprofit foundation "Alphabet Soup" to help select applicants for funding with the best chance of success in their ventures. The neural network model uses the features in the dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

# Results:
Using bulleted lists and images to support your answers, address the following questions:

## Data Preprocessing
1. What variable(s) are the target(s) for your model?<br/>
   The target variable is the "IS_SUCCESSFUL" column from the application_df
   
2. What variable(s) are the features for your model?<br/>
   The features are all of the other columns that remain in the dataframe after the target column("IS_SUCCESSFUL") is dropped
 
3. What variable(s) should be removed from the input data because they are neither targets nor features?<br/>
   The "EIN" and "NAME" columns should be removed

## Compiling, Training, and Evaluating the Model
1. How many neurons, layers, and activation functions did you select for your neural network model, and why?<br/>
   Initially, I selected two hidden layers, with 80 units for the first hidden layer and 30 units for the second hidden layer. After some reading (article titled "Activation    Functions in Neural Networks [12 Types & Use Cases]" on v7labs.com), I decided to use the ReLU activation function for both hidden layers. For the output layer, I used       the Sigmoid activation function.
   
2. Were you able to achieve the target model performance?<br/>
   I was not able to achieve the target accuracy of 75%
   
3. What steps did you take in your attempts to increase model performance?<br/>
   After the initial pass, I tried several methods to optimize the model including: dropping additional columns from the dataframe, adjusting the number of units in the         hidden layers, changing the activation function(s) of the hidden layers, as well as adding a third hidden layer.
   
# Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then       explain your recommendation.
  Overall, the model was approximately 73% accurate. One additional approach that could be tried to increase model accuracy would be to sort the initial data by further        binning. Additionally, more hidden layers could be added to increase the power of the model. Finally, additional activation functions could be attempted for each of the      hidden layers.
