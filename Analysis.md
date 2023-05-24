Overview of the analysis: Explain the purpose of this analysis.

Results: Using bulleted lists and images to support your answers, address the following questions:

## Data Preprocessing

**What variable(s) are the target(s) for your model?**
    - IS_SUCCESSFUL is the y-variable for this data, known as the target. 

**What variable(s) are the features for your model?**
    - X Variables = APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT

**What variable(s) should be removed from the input data because they are neither targets nor features?**
    - EIN and Name should be removed from the data. They are not the target and they are not a feature of this dataset, and therefore is not relevent in this nueral network model. 

## Compiling, Training, and Evaluating the Model

**How many neurons, layers, and activation functions did you select for your neural network model, and why?**

Optimization Attempt 1:

![]("C:\Users\b_ber\OneDrive\Desktop\Bootcamp\Module21\deep-learning-challenge\Resources\Attempt 1 . columns removal.jpg")

![]("C:\Users\b_ber\OneDrive\Desktop\Bootcamp\Module21\deep-learning-challenge\Resources\X y Variables.jpg")

![]("C:\Users\b_ber\OneDrive\Desktop\Bootcamp\Module21\deep-learning-challenge\Resources\nn1 keras model.jpg")

![]("C:\Users\b_ber\OneDrive\Desktop\Bootcamp\Module21\deep-learning-challenge\Resources\nn1 evaluation.jpg")

Optimization Attempt 2:

![]("C:\Users\b_ber\OneDrive\Desktop\Bootcamp\Module21\deep-learning-challenge\Resources\Attempt 1 . columns removal.jpg")

![]("C:\Users\b_ber\OneDrive\Desktop\Bootcamp\Module21\deep-learning-challenge\Resources\X y Variables.jpg")

![]("C:\Users\b_ber\OneDrive\Desktop\Bootcamp\Module21\deep-learning-challenge\Resources\nn1 keras model.jpg")

![]("C:\Users\b_ber\OneDrive\Desktop\Bootcamp\Module21\deep-learning-challenge\Resources\nn1 evaluation.jpg")

Optimization Attempt 3:

![]("C:\Users\b_ber\OneDrive\Desktop\Bootcamp\Module21\deep-learning-challenge\Resources\nn2 columns.jpg")

![]("C:\Users\b_ber\OneDrive\Desktop\Bootcamp\Module21\deep-learning-challenge\Resources\X y Variables.jpg")

![]("C:\Users\b_ber\OneDrive\Desktop\Bootcamp\Module21\deep-learning-challenge\Resources\nn2 keras model.jpg")

![]("C:\Users\b_ber\OneDrive\Desktop\Bootcamp\Module21\deep-learning-challenge\Resources\nn2 evaluation.jpg")



**Were you able to achieve the target model performance?**
    - No, I was not able to acheive a target model performance. When I took additional columns out of the dataset it caused the accuracy to lower. When I kept the columns the same as the original model, but added hidden layers and neurons it increased slightly, but not by much. Only a percent or two. 

**What steps did you take in your attempts to increase model performance?**

Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.