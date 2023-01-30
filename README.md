## Alphabet Soup’s business Analysis

## Purpose of this analysis

Based on binary classifier with machine learning model to predict whether applicants will be successful if funded by Alphabe Soup. Build the own machine learning model and improve the model accuracy. 

## Result( how to increase accuracy)
*What variable(s) are considered the target(s) for your model?
I check the "successful" in dataset, this means the applicants will be successful recived the funded from Alphabe Soup.

*What variable(s) are considered to be the features for your model?
 Features: Every Columns except"IS_SUCCESSFUL" 

*What variable(s) are neither targets nor features, and should be removed from the input data?
Remove" EIN" and "Name" columns, since will not improve the accuracy. 



Data Preprocessing,Four steps tring to achieve the accuracy target 75% / 
* Drop more noisy variable. original, I only drop "EIN", "NAME" => The accuracy only  53%. I drop two more noisy variable " STATUS" and "ask amount", I am able to increase the accuracy higher to 54%
![small improvment]
https://github.com/violetqq0221/Neural_Network_Charity_Analysis/blob/main/Final%20Result_%20Accuracy%2065%25.PNG
Compiling, Training and Evaluating the Model
* Add additional neurons to hidden layers. The intial I start 8 neurons on hidden layer 1 and 4 neuron on hidden layer2. The result of accuracy only 65% . I tried few time, different neurons combimation. The finally I add 100 neurons on first hidden layer and 30 neurons on second hidden layer, the accuracy of the result able to achive 70.4% 
![After Optimization ](https://github.com/violetqq0221/Neural_Network_Charity_Analysis/blob/main/Final%20Result_%20Accuracy%2065%25.PNG)
![After Optimization ](https://github.com/violetqq0221/Neural_Network_Charity_Analysis/blob/main/Final%20Result_%20Accuracy%2070.4%25.PNG)
  
## Summary:
This deep learning model is 70.4% after attemping optimization. Try to change activation function, and also train the data with more epoches. The accuracy didn't see any significant improvment. Changing hidden layer neuron can see the some improvement of accuracy. 
![Summary ](https://github.com/violetqq0221/Neural_Network_Charity_Analysis/blob/main/Module.PNG)
