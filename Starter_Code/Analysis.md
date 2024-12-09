# Analysis Report

## Data Preprocessing
    * What Variable(s) are the target(s) for your model?
        The target for the model is the "Is_Successful" column. 
    * What Variable(s) are the features for your model?
        The features of this model are the Name, Application, Type, Affiliation, Classification, Use_Case, Organization, Income_Amt, Special_Considerations, Status, and Ask_Amt.
    * WHat Variable(s) should be removed from the input data because they are neither tagets nor features?
        EIN was dropped because the numbers could confuse the system into thinking its significant. 


## Compiling, Training, and Evaluating the Model
    * How many neurons, layers, and activation functions did you select for your neural network model, and why?
        In this model there are 3 hidden layers, one more then the previous model. This was done to see if adding an extra layer would increase the accuracy to atleast 75%. The first activation function was 'relu' but the 2nd and 3rd were 'sigmoid' and the output function was 'sigmoid'.
    * Were you able to achieve the target model performance?
        Yes
    * What steps did you take in your attempts to increase model performance?
        It reuqired adding a third layer and using the "sigmoid" activation function for the 2nd and 3rd layer. 


## Summary

    Overall we were able to increase the accuracy above 75%. Applicants have a 80% chance of being successful if they have the following:
        * The NAME of the applicant appears more than 5 times.
        * The type of APPLICATION is >500
        * The application has the following CLASSIFICATION is >1000
    A good model to recommend is the Random Forest model. 