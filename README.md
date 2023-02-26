# Neural_Network_Charity_Analysis

## Objective

The purpose of this challenge is to utilize our knowledge of machine learning and neural networks, using features in the provided dataset to assist our client in creating a binary classifer that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

This will be accomplised by completing three technical analysis components and a written report.  The technical analysis includes:
- Preprocessing Data for a Neural Network Model
- Compile, Train, and Evaluate the Model
- Optimize the Model

## Results 

### Data Preprocessing

![](Resources/Target_Feature_Column.png)

The client requested we answer the following questions:

Q1. What variable(s) are considered the target(s) for your model?

*A1. The IS_SUCCESSFUL column indicates that a charity has been successfully funded by AlphabetSoup, thereby this column will be considered a target for the model.*

Q2. What variable(s) are considered to be the features for our model?

*A2. The IS_SUCCESSFUL column will also be the feature chosen for this dataset.*

Q3. What variable(s) are neither targets nor features, and should be removed from the input data?

*A3. The EIN and NAME columns are neither targets nor features for this dataset and were removed from the input data.*

### Compiling, Training, and Evaluating the Model

**Initial Model Results**

![](Resources/Attempt0.png)

![](Resources/Attempt0a.png)

The client requested we answer the following questions:

Q1. How many nuerons, layers,and activation funtions did you select for your neural network model, and why?

*A1. In the initial neural network model, I referenced a previous successful example as a starting place and began with three layers. The first layer had 80 neurons with a sigmoid activation.  The second layer had 20 neurons with a relu activation, and the final layer utilized a linear activation.*

Q2. Were you able to achieve the target model performances?

*A2. The initial neural network model yielded a 71.6% accuracy.  Although efforts were made to optimize the model, the highest accuracy achieved was 72.4%.*

Q3. What steps did you take to try and increase model performance?

*A3. The steps taken to try and increase model performance are documented below:

-Optimization 1: Added a third layer (for a total of 4) with 10 neurons and a relu activation. Accuracy: 72.4%
-Optimization 2: Reduced back to three total layers, changed the neurons to 8,5,1 and changed the output layer activation from linear to sigmoid. Accuracy: 72.4%
-Optimization 3: Maintained the same number of layers and neurons as Optimization 2, however, changed the output layer activation to linear. Accuracy: 46.7%
-Optimization 4: Returned the output layer back to sigmoid, kept three layers and increased the neurons to 12, 6, 1. Accuracy: 72.1%

**Optimization Results**

*Optimization 1*

![](Resources/Attempt1.png)

![](Resources/Attempt1a.png)

*Optimization 2* 

![](Resources/Attempt2.png)

![](Resources/Attempt2a.png)

*Optimization 3*

![](Resources/Attempt3.png)

![](Resources/Attempt3a.png)

*Optimization 4*

![](Resources/Attempt4.png)

![](Resources/Attempt4a.png)

### Summary
In summary, Optimization effort 1 yielded the highest accuracy at 72.4%.  Future modeling may benefit from utilizing the random forest classifier, as it is less influenced by outliers.

