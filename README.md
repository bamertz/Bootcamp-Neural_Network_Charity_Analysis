# Neural_Network_Charity_Analysis

## Overview

The purpose of this project is to use deep-learning neural networks by using the TensorFlow platform in Python to analyze and classify charitable donations from the data provided by Alphabet Soup. The data consists of 34,000 organizations that have received funding. 

* Deliverable 1: Preprocessing Data for a Neural Network Model
* Deliverable 2: Compile, Train, and Evaluate the Model
* Deliverable 3: Optimize the Model
* Deliverable 4: A Written Report on the Neural Network Model


## Results

### Deliverable 1: Preprocessing Data for a Neural Network Model

1. What variable(s) are considered the target(s) for your model?
  
  * IS_SUCCESSFUL - Whether or not the charity donation was used effectively.

2. What variable(s) are considered to be the features for your model?

  * APPLICATION_TYPE
  * AFFILIATION
  * CLASSIFICATION
  * USE_CASE
  * ORGANIZATION
  * STATUS
  * INCOME_AMT
  * SPECIAL_CONSIDERATIONS
  * ASK_AMT
 
  These features have been counted, had bins created, and standardized.

3. What variable(s) are neither targets nor features, and should be removed from the input data?

 * EIN
 * NAME
  
  These variables are categorical information and were removed from the input data.

### Deliverable 2: Compile, Train, and Evaluate the Model

1. How many neurons, layers, and activation functions did you select for your neural network model, and why?

  * 2 LAYERS
  * 1ST LAYER - 80 NEURONS
  * 2ND LAYER - 30 NEURONS
  * RELU ACTIVATION FUNCTION
  * TOTAL PARAMS - 5,901
  * TRAINABLE PARAMS - 5,901

2. Were you able to achieve the target model performance?

  * NO
  * LOSS - 0.6381
  * ACCURACY - 0.6856 WHICH IS LESS THAN 75%

### Deliverable 3: Optimize the Model

3. What steps did you take to try and increase model performance?

  * OPTIMIZATION ATTEMPT 1:
        * 1ST LAYER - 100 NEURONS, RELU FUNCTION
        * 2ND LAYER - 75 NEURONS, SIGMOID FUNCTION
        * 3RD LAYER - 50 NEURONS, SIGMOID FUNCTION
        * OUTPUT LAYER - SIGMOID FUNCTION
        * LOSS - 0.6920
        * ACCURACY - 0.5255
  
  * OPTIMIZATION ATTEMPT 2:
        * 1ST LAYER - 150 NEURONS, RELU FUNCTION
        * 2ND LAYER - 100 NEURONS, RELU FUNCTION
        * OUTPUT LAYER - SIGMOID FUNCTION
        * LOSS - 0.6920
        * ACCURACY - 0.5255

  * OPTIMIZATION ATTEMPT 3:
        * 1ST LAYER - 160 NEURONS, TANH FUNCTION
        * 2ND LAYER - 130 NEURONS, TANH FUNCTION
        * OUTPUT LAYER - SIGMOID FUNCTION
        * LOSS - 0.5726
        * ACCURACY - 0.7236

## Summary

* The deep learning neural network model only reached an accuracy of 72.36% which was less than the required 75%. The most effective model occured after the 3rd optimatization attempt which also had the lowest loss of 52.76%. Potentially, a 4th optimization and using the TANH function as an output layer or increasing the Neurons may yield the desired results. Supervised machine learning models could be used or other classification models like the balanced random forest classifer which would generate a classified output worth comparing to the deep learning model.

* Note: Deliverable 4: A Written Report on the Neural Network Model is this README File.
