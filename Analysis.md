Overview of the analysis: Explain the purpose of this analysis.

Results: Using bulleted lists and images to support your answers, address the following questions:

## Data Preprocessing

**What variable(s) are the target(s) for your model?**

- IS_SUCCESSFUL is the y-variable for this data, known as the target. 

**What variable(s) are the features for your model?**
    
- X Variables = APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT

![](https://github.com/bernbr/deep-learning-challenge/blob/83cb7d4c8b8097b251b816d40f2918a70a6bffff/Images/X%20y%20Variables.jpg?raw=true)

**What variable(s) should be removed from the input data because they are neither targets nor features?**
    
- EIN and Name should be removed from the data. They are not the target and they are not a feature of this dataset, and therefore is not relevent in this nueral network model. 

![](https://github.com/bernbr/deep-learning-challenge/blob/83cb7d4c8b8097b251b816d40f2918a70a6bffff/Images/Drop%20Columns.jpg?raw=true)

## Compiling, Training, and Evaluating the Model

**How many neurons, layers, and activation functions did you select for your neural network model, and why?**

Optimization Attempt 1:
**Model 1:** 
![](https://github.com/bernbr/deep-learning-challenge/blob/83cb7d4c8b8097b251b816d40f2918a70a6bffff/Images/nn1%20model.jpg?raw=true)

**Structure**
![](https://github.com/bernbr/deep-learning-challenge/blob/83cb7d4c8b8097b251b816d40f2918a70a6bffff/Images/Model%201%20Structure.jpg?raw=true)

**Training**
![](https://github.com/bernbr/deep-learning-challenge/blob/83cb7d4c8b8097b251b816d40f2918a70a6bffff/Images/Model%201%20Training%20.jpg?raw=true)

**Evaluation**
![](https://github.com/bernbr/deep-learning-challenge/blob/83cb7d4c8b8097b251b816d40f2918a70a6bffff/Images/Model%201%20Evaluation.jpg?raw=true)

Optimization Attempt 2:
**Model 2:** 
![](https://github.com/bernbr/deep-learning-challenge/blob/83cb7d4c8b8097b251b816d40f2918a70a6bffff/Images/nn2%20model.jpg?raw=true)

**Structure**
![](https://github.com/bernbr/deep-learning-challenge/blob/83cb7d4c8b8097b251b816d40f2918a70a6bffff/Images/Model%202%20Structure.jpg?raw=true)

**Training**
![](https://github.com/bernbr/deep-learning-challenge/blob/83cb7d4c8b8097b251b816d40f2918a70a6bffff/Images/Model%202%20Training.jpg?raw=true)

**Evaluation**
![](https://github.com/bernbr/deep-learning-challenge/blob/83cb7d4c8b8097b251b816d40f2918a70a6bffff/Images/Model%202%20Evaluation.jpg?raw=true)


Optimization Attempt 3:
**Model 3:** 
![](https://github.com/bernbr/deep-learning-challenge/blob/83cb7d4c8b8097b251b816d40f2918a70a6bffff/Images/nn3%20model.jpg?raw=true)

**Structure**
![](https://github.com/bernbr/deep-learning-challenge/blob/83cb7d4c8b8097b251b816d40f2918a70a6bffff/Images/Model%203%20Structure.jpg?raw=true)

**Training**
![](https://github.com/bernbr/deep-learning-challenge/blob/83cb7d4c8b8097b251b816d40f2918a70a6bffff/Images/Model%203%20Training.jpg?raw=true)

**Evaluation**
![](https://github.com/bernbr/deep-learning-challenge/blob/83cb7d4c8b8097b251b816d40f2918a70a6bffff/Images/Model%203%20Evaluation.jpg?raw=true)





**Were you able to achieve the target model performance?**
    - No, I was not able to acheive a target model performance. When I took additional columns out of the dataset it caused the accuracy to lower. When I kept the columns the same as the original model, but added hidden layers and neurons it increased slightly, but not by much. Only a percent or two. 

**What steps did you take in your attempts to increase model performance?**

Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.