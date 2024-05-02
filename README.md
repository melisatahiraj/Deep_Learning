# Deep Learning

### Preprocess the Data
* Create a dataframe containing the *charity_data.csv* data , and identify the target and feature variables in the dataset
* Drop the *EIN* and *NAME* columns
![1st_model_drop_columns](https://github.com/melisatahiraj/deep-learning-challenge-21/assets/147450801/9ccd6bab-914a-4a2a-a897-bb8866c43588)
* Determine the number of unique values in each column
* For columns with more than 10 unique values, determine the number of data points for each unique value
* Create a new value called *Other* that contains rare categorical variables
* Create a feature array, *X*, and a target array, *y* by using the preprocessed data
![is_successful_adummies](https://github.com/melisatahiraj/deep-learning-challenge-21/assets/147450801/645dd209-84de-4f16-8907-72f2f3750541)
* Split the preprocessed data into training and testing datasets
* Scale the data by using a *StandardScaler* that has been fitted to the training data

### Compile, Train and Evaluate the Model
* Create a neural network model with a defined number of input features and nodes for each layer
* Create hidden layers and an output layer with appropriate activation functions
![1st_model_nodes](https://github.com/melisatahiraj/deep-learning-challenge-21/assets/147450801/b936263c-a036-4477-8914-bff45cf494d8)
* Check the structure of the model
* Compile and train the model
* Evaluate the model using the test data to determine the loss and accuracy
![1st_model_accr](https://github.com/melisatahiraj/deep-learning-challenge-21/assets/147450801/847d5bb7-e88d-42d5-933a-466f96e6f8ce)
* Export your results to an HDF5 file named *AlphabetSoupCharity.h5*

### Optimize the Model
* Repeat the preprocessing steps in a new Jupyter notebook
* Create a new neural network model, implementing at least 3 model optimization methods
![opt_model_nodes](https://github.com/melisatahiraj/deep-learning-challenge-21/assets/147450801/75c95eea-1b0d-4866-9c32-df05b841d1ff)
![opt_model_accr](https://github.com/melisatahiraj/deep-learning-challenge-21/assets/147450801/4c554527-bfdc-4ff2-bbd3-a761fc74461e)
* Save and export your results to an HDF5 file named *AlphabetSoupCharity_Optimization.h5*

### Write a Report on the Neural Network Model
* Write an analysis that includes a title and multiple sections, labeled with headers and subheaders saved in *Report on the Neural Network Model*
* Format images in the report so that they display correction
* Explain the purpose of the analysis
* Answer all 6 questions in the results section
* Summarize the overall results of your model
* Describe how you could use a different model to solve the same problem, and explain why you would use that model

# References
IRS. Tax Exempt Organization Search Bulk Data Downloads. https://www.irs.gov/
