### Charity Funding Predictor Report


## Overview
The purpose of this analysis is to create an algorithm for Alphabet Soup foundation that can predict whether or not applicants for funding will be successful. 


## Results
*  Data Preprocessing 
    * What variable(s) are considered the target(s) for your model?
        * The target of the model was if the applicants were successful which was listed in column “IS_SUCCESSFUL”
    * What variable(s) are considered to be the features for your model?
        * All columns except for EIN, NAME and IS_SUCCESSFUL were considered as features for the model except for last attempt to boost, which only included APPLICATION_TYPE and CLASSIFICATION columns.
    * What variable(s) are neither targets nor features, and should be removed from the input data?
        * The columns EIN and NAME were removed from the data since they did not add any values.
* Compiling, Training, and Evaluating the Model 
    * How many neurons, layers, and activation functions did you select for your neural network model, and why?
        * The initial model had 3 layers including output layer and the last model had 5 layers including output layer. They both used mix of ReLU and sigmoid in attempt to improve accuracy 
    * Were you able to achieve the target model performance?
        * The goal of the model was to achieve over 75% accuracy, but this model could only achieve 72.5% accuracy
    * What steps did you take to try and increase model performance?
        * In attempts to increase the model performance, more layers were added with various activation functions and cleaned data to exclude applicant types and classifications marked as ‘other’.

## Summary 
In summary, with the current model, we can accurately predict the success rate at over 70%. Since the label we used were ‘yes’ or ‘no’, the binary classification would work best for this data.
