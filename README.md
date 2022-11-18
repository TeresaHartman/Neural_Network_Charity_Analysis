# Neural_Network_Charity_Analysis

## Overview of the analysis: Explain the purpose of this analysis.
I am trying to analyze the impact of each donation of AlphabetSoup and vet potential recipients. This helps ensure that the foundations money is being used effectively, as not every donation the company makes is impactful. This analysis done here will be able to predict which organizations are worth donating too and which will be too high risk. To help with the task above, I have designed and trained a deep learning neural network which will evaluate all types of input data.   

## Results: 
### Data Preprocessing
* What variable(s) are considered the target(s) for your model?
  * The target for this module is whether the donation was considered successful or not. 
* What variable(s) are considered to be the features for your model?
  * The variables for this model are 
    * The type of application
    * The affiliated sector of industry
    * The government organization classification
    * Use case for funding
    * Organization type
    * Active status
    * Income classification
    * Special consideration for application
    * Funding amount requested
* What variable(s) are neither targets nor features, and should be removed from the input data?
  * The EIN and NAME columns were only used for identification columns and removed from the input data.  

### Compiling, Training, and Evaluating the Model
* How many neurons, layers, and activation functions did you select for your neural network model, and why?
  * The initial neural network model used two hidden layers, the first with 80 neurons and the second with 30 neurons. 
* Were you able to achieve the target model performance?
  * After trying several different approaches, I was unable to achieve the target performance of 75%. 
* What steps did you take to try and increase model performance?
 * Several different methods were attempted to improve the accuracy rating. The first thing observed was that in almost every test run, there wasn't any advantage to running over 25 epochs. Other attempts including increasing and decreasing the number of neurons in each layer, as well as, increasing the number of layers to 3. After noticing those weren't improving the accuracy rating, the next attempt was to change the values of the bucketing in the application type, and classification categories. None of these methods were able to improve the accuracy rating of over 53%. At most, the only thing that was able to be improved as the loss rating. I also looked at all the quantitative values to see if there were any outliers that could be affecting the results. The only actual variable worth investigating was the ask amount values, and while those are definitely skewed, there weren't any outliers that could be removed to adjust the data. 
 
## Summary: 
The best predictive accuracy rating that was able to be achieved was 0.53 with a loss of 0.69. Since this is only able to predict successful donations a little over half the time, I wouldn't suggest to use the neural network to predict accuracy with all input variables considered at once. Instead, I would recommend trying to separate some of the input factors into similar categories and then try to rerun the model. Since the data was so skewed, my first suggestion would be to separate the ask amount column into two different categories, one containing smaller amounts and one containing much higher amounts.
