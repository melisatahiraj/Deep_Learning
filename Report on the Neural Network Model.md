# Report on the Neural Network Model

## Overview
We are analyzing the data for Alphabet Soup, a nonprofit foundation, to help them choose which applicants are most likely to succeed if funded. We will use the data they provided to create a machine learning tool that can predict whether an applicant will be successful with their funding. The dataset contains more than 34,000 organizations that have received funding from Alphabet Soup in the past.

## Results
### Data Preprocessing

* <b> What variable(s) are the target(s) for your model? </b>   
The target for our model is the column "IS SUCCESSFUL" represented by the variable "y".

* <b> What variable(s) are the features for your model? </b>    
The features for our model are all the columns except "IS SUCCESSFUL" which is dropped in the variable "X".

* <b> What variable(s) should be removed from the input data because they are neither targets nor features? </b>    
In the first model the variables that I removed from the input data because they are neither targets nor features are "EIN" and "NAME". Whereas, in the optimization model I am also dropping the "SPECIAL_CONSIDERATIONS" column because they are neither targets nor features and it improves the model's performance.

### Compiling, Training, and Evaluating the Model

* <b> How many neurons, layers, and activation functions did you select for your neural network model, and why? </b>
  #### 1st Model

  Hidden Layer 1 = 20 -- Activation = ReLu    
  I used ReLu in the 1st layer because it allows the network to learn faster and it helps the model capture complex patterns.

  Hidden Layer 2 = 10 -- Activation = ReLu    
  I used ReLu in the 2nd layer again for similar reasons. By using ReLu again it continues to capture the complex patterns effectively.

  Output Layer = 1 -- Activation = Sigmoid    
  I used Sigmoid in the output layer because it is the most useful method for binary classification. Sigmoid is well-suited for the purpose of squashing the output to the range of 0 and 1, representing the probability of belonging to one class. 

  #### Optimization Model

  Hidden Layer 1 = 70 -- Activation = ReLu   
  I used ReLu in the 1st layer because it allows the network to learn faster and it helps the model capture complex patterns.

  Hidden Layer 2 = 35 -- Activation = ReLu   
  I used ReLu in the 2nd layer again for similar reasons. By using ReLu again it continues to capture the complex patterns effectively.
  
  Output Layer = 1 -- Activation = Sigmoid   
  I used Sigmoid in the output layer because it is the most useful method for binary classification. Sigmoid is well-suited for the purpose of squashing the output to the range of 0 and 1, representing the probability of belonging to one class.

       
* <b> Were you able to achieve the target model performance? </b>    
  In the 1st Model I was able to achieve only 70.9% model accuracy.    
  In the Optimization Model I was able to achieve the target model performance with 75.3% accuracy.

* <b> What steps did you take in your attempts to increase model performance? </b>    
  To increase the model performance, firstly I dropped another column in the optimization model. Secondly, without changing the number of layers, I increased the number of nodes for each layer to enable the model to capture more intricate patterns in   the data. Lastly, I extended the training duration by doubling the number of epochs to allow the model more opportunity to learn from the data. These changes were successful in increasing the model's accuracy. 

## Summary

Overall, the deep learning models developed for predicting the success of funding applicants for Alphabet Soup yielded promising results. The first model achieved a respectable accuracy of 70.9%, while the optimization model significantly improved performance to reach the target accuracy of 75.3%. By strategically adjusting the architecture of the neural network, including increasing the number of nodes in each hidden layer and extending the training duration, the optimization model effectively captured more complex patterns in the data, resulting in better predictions.

A different approach to solving this classification problem is Random Forest which handles non-linear relationships and interactions between features effectively. Random Forest is also relatively easy to interpret, providing insights into which features are most influential in predicting funding success, aiding decision-making for Alphabet Soup.
