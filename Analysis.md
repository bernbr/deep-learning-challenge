# **Overview of the analysis:** 

The purpose of this analysis is to determine whether or not a loan is good or bad based on previous loans features. 

# **Results:** 

### Data Preprocessing

**What variable(s) are the target(s) for your model?**

- IS_SUCCESSFUL is the y-variable for this data, known as the target. 

**What variable(s) are the features for your model?**
    
- X Variables = APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT

![](https://github.com/bernbr/deep-learning-challenge/blob/83cb7d4c8b8097b251b816d40f2918a70a6bffff/Images/X%20y%20Variables.jpg?raw=true)

**What variable(s) should be removed from the input data because they are neither targets nor features?**
    
- EIN and Name should be removed from the data. They are not the target and they are not a feature of this dataset, and therefore is not relevent in this nueral network model. 

![](https://github.com/bernbr/deep-learning-challenge/blob/83cb7d4c8b8097b251b816d40f2918a70a6bffff/Images/Drop%20Columns.jpg?raw=true)

### Compiling, Training, and Evaluating the Model

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

- No, I was not able to acheive a target model performance. When I took additional columns out of the dataset it caused the accuracy to lower, not included in the 3 optimization attempts. I decided to leave them the columns as they were in the instructions, for the final optimization attempts. When additional columns were taken out, the data dropped to the low 60s. 

- With the final optimization models, I was able to get close to .73. Which was slightly higher, but not by much. With more time and resources I think I could have found a model that fit with activations of tanh and sigmoids. However, with many different attempts, both shown and not shown, I was not able to get over .73 for accuracy.

**What steps did you take in your attempts to increase model performance?**

- Some steps I attempted were removing additional columns. Some additional columns I attempted to remove in my preprocessing, which are not documented, were affiliation, classification, and organization. Removal of some or all of those resulted in significatly lower accuracy scores. 

- Next, I wanted to try various activation codes and units. In the starter code it started with relu activation and a little less than double the input for the units. 

- I wanted to see what various combinations to see what various activations, units, and hidden nodes did to the data. With the outputs that came out of the models, I determined that relu was probably a likely contender, seeing as the accuracy was the highest with relu. 

# **Summary:** 

- With the features provided the data models I worked through could only get to .74 accuracy. I think use of a keras-tuner would be helpful in this scenario to determine if this tool can get a higher accuracy, or is it only three-fourths effective. 

- I would recommend trying to a support vector machine classifier. A SVM classifer will help find the hyperplane between the two groups of data. This would hopefully help determine classification of future data points by determining if the output of a linear function is 1 or -1, and then put the data point in the corresponding class. In this case it would classify the data point as a high risk loan or a good loan. 
