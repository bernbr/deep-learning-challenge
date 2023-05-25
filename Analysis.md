Overview of the analysis: Explain the purpose of this analysis.

Results: Using bulleted lists and images to support your answers, address the following questions:

## Data Preprocessing

**What variable(s) are the target(s) for your model?**
    - IS_SUCCESSFUL is the y-variable for this data, known as the target. 

**What variable(s) are the features for your model?**
    - X Variables = APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT

![]("Images/X y Variables.jpg")

**What variable(s) should be removed from the input data because they are neither targets nor features?**
    - EIN and Name should be removed from the data. They are not the target and they are not a feature of this dataset, and therefore is not relevent in this nueral network model. 

![]("Images/Drop Columns.jpg")

## Compiling, Training, and Evaluating the Model

**How many neurons, layers, and activation functions did you select for your neural network model, and why?**

Optimization Attempt 1:
**Model 1:** 
![]("Images/nn1 model.jpg")

**Structure**
![]("Images/Model 1 Structure.jpg")

**Training**
![]("Images/Model 1 Training .jpg")

**Evaluation**
![][https://github.com/bernbr/deep-learning-challenge/blob/034ce3bfb4141212846428350a8314a702cba176/Images/Model%201%20Evaluation.jpg]


Optimization Attempt 2:
**Model 2:** 
![]("Images/nn2 model.jpg")

**Structure**
![]("Images/Model 2 Structure.jpg")

**Training**
![]("Images/Model 2 Training.jpg")

**Evaluation**
![]("Images/Model 2 Evaluation.jpg")


Optimization Attempt 3:
**Model 3:** 
![]("Images/nn3 model.jpg")

**Structure**
![]("Images/Model 3 Structure.jpg")

**Training**
![]("Images/Model 3 Training.jpg")

**Evaluation**
![]("Images/Model 3 Evaluation.jpg")





**Were you able to achieve the target model performance?**
    - No, I was not able to acheive a target model performance. When I took additional columns out of the dataset it caused the accuracy to lower. When I kept the columns the same as the original model, but added hidden layers and neurons it increased slightly, but not by much. Only a percent or two. 

**What steps did you take in your attempts to increase model performance?**

Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.