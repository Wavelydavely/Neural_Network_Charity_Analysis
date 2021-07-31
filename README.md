# Neural_Network_Charity_Analysis

Overview of the analysis:

We are looking to weed out funding for charities which do not use their revenue efficiently. With this analysis, we are hoping to create a predictive model to determine which factors lead to efficient revenue use.

Results:

Data Preprocessing
What variable(s) are considered the target(s) for your model?
Our target variable is the column IS_SUCCESSFUL.

What variable(s) are considered to be the features for your model?
The challenge of this analysis is to determine which potential features are meaningful. Our most accurate model is using every column except 'EIN', 'NAME', 'USE_CASE', 'CLASSIFICATION', and 'APPLICATION_TYPE', but this model is still not as accurate as we would like.

What variable(s) are neither targets nor features, and should be removed from the input data?
From the input data, we have removed 'EIN', 'NAME', 'USE_CASE', 'CLASSIFICATION', and 'APPLICATION_TYPE'. These variables seem to have little correlation with the efficient use of charity funds.

Compiling, Training, and Evaluating the Model
How many neurons, layers, and activation functions did you select for your neural network model, and why?
We experimented using two and three layers, using different combinations of 80, 50, 30, and 25 neurons per node. We used Relu for the hidden nodes and Sigmoid for the output.

Were you able to achieve the target model performance?
We ultimately failed to achieve target model performance in three attempts.

What steps did you take to try and increase model performance?
We tried to eliminate superfluous features of our original model. We also experimented with different numbers of layers and neurons per layer.

Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.

AlphabetSoupCharity_Optimzation.h5
'EIN', 'NAME', 'USE_CASE', 'CLASSIFICATION', 'APPLICATION_TYPE' variables removed
Loss: 1.5839394330978394, Accuracy: 0.6594752073287964

AlphabetSoupCharity_Optimzation(0).h5
'EIN', 'NAME', 'USE_CASE', 'CLASSIFICATION', 'APPLICATION_TYPE'variables removed
Third hidden layer w/50 nodes
Loss: 0.6877241730690002, Accuracy: 0.5890378952026367


AlphabetSoupCharity_Optimzation(1).h5
hidden_nodes_layer1 = 50
hidden_nodes_layer2 = 30
Loss: 0.6909811496734619, Accuracy: 0.6606413722038269

