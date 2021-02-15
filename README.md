# Neural Network Charity Analysis
## Overview of the analysis
The objective of this project is to analyse past funding results to determine if the applicant organization will be able to successfully reach their goals. The analysis uses knowledge of Machine learning and neural networks to create a binary classifier that is capable of predicting the success of a funding project.

Technologies

- ```Python 3.8```

- ```Scikit-Learn library```

- ```TensorFlow v2.4.0 library```

Data Source

```charity_data.csv```

## Results  

Data Preprocessing
#### What variable(s) are considered the target(s) for your model?
```Target variable(s): IS_SUCCESSFUL```

#### What variable(s) are considered to be the features for your model?
```Features variable(s): APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT, STATUS```

#### What variable(s) are neither targets nor features, and should be removed from the input data?

The ```EIN``` and ```NAME``` columns are removed since they do not play a part in the project success.

### Compiling, Training, and Evaluating the Model

#### How many neurons, layers, and activation functions did you select for your neural network model, and why?

![Neuron layer activation functions.png](https://github.com/smj452/Neural_Network_Charity_Analysis/blob/main/Resources/Neuron%20layer%20activation%20functions.png)

The final model selected consists of 3 hidden layers with 50, 20 and 3 neurons each. The activation function used for the middle layers was relu and for the output layer is sigmoid.

#### Were you able to achieve the target model performance?

No, the highest accuracy for the model was 72%. Our target was 75%.

#### What steps did you take to try and increase model performance?

- Used different activation functions for the hidden layers.
- Changed the number of neurons to get the highest accuracy.
- Change model's weights to be saved every 5 epochs.

## Summary


Even after several attempts we were not able to achieve the target accuracy level of 75%.
The final model selected consisted of 3 hidden layers with 50, 20 and 3 neurons each. The activation function used for the middle layers was relu and for the output layer is sigmoid.

- The Random forest classifiers model can be used to solve the classification problem. Both output and feature selection of random forest models are easy to interpret, and they can easily handle outliers and nonlinear data.
