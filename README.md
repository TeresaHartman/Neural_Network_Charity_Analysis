# Neural_Network_Charity_Analysis

## Overview of the analysis: Explain the purpose of this analysis.
I am trying to analyize the impact of each donation of AlphabetSoup and vet potential recpeients. This helps ensure that the foundations money is being used effitively, as not every donation the company makes is impactful. This analysis done here will be able to predict which oranizations are worth donating too and which will be too high risk. To help with the task above, I have designed and trained a deep learning neural network which will evaluate all types of input data.  

## Results: 
### Data Preprocessing
* What variable(s) are considered the target(s) for your model?
  * The target for this module is whether the donation was considered successful or not. 
* What variable(s) are considered to be the features for your model?
  * The variables for this model are 
    * The type of application
    * The affiliated sector of industry
    * The government organization classification
    * Use case for dungind
    * Organization type
    * Active status
    * Income classification
    * Special consideration for application
    * Funding amount requested
* What variable(s) are neither targets nor features, and should be removed from the input data?
  * The EIN and NAME columns were only used for indentification columns and removed from the input data.  

### Compiling, Training, and Evaluating the Model
* How many neurons, layers, and activation functions did you select for your neural network model, and why?
  * 
* Were you able to achieve the target model performance?
  * After trying several different approaches, I was unable to get higher than the initial 
* What steps did you take to try and increase model performance?

## Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.
