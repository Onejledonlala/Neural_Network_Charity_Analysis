# Neural_Network_Charity_Analysis

## Overview of the analysis

This analysis gives insight of machine learning and neural networks, features used in the provided dataset to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. The dataset is a CSV containing more than 34,000 organizations with a number of columns that capture metadata about each organization.

## Results

Below are lists and images to show the process to machine learning and neural networks

#### - Data Preprocessing

  - The variable considered the target for the model is **IS_SUCCESSFUL**
  
  - The variables considered as features for the model are:
    - APPLICATION_TYPE          
    - AFFILIATION               
    - CLASSIFICATION            
    - USE_CASE                  
    - ORGANIZATION             
    - INCOME_AMT                
    - SPECIAL_CONSIDERATIONS 
    ![image](https://user-images.githubusercontent.com/78067427/123911586-f7e8c800-d949-11eb-9614-f85d176788d8.png)
   
   -  The variables considered to be neither targets nor features, and should be removed from the input data are 
    ![image](https://user-images.githubusercontent.com/78067427/123912238-c7edf480-d94a-11eb-8377-143728fa1c5f.png)
   
#### - Compiling, Training, and Evaluating the Model

   - The model has 44 features, 2 hidden node layers of 80 and 50 as relu being the activation fucktion which gives parameters of 3520 and 4050 respectively. It also has the output layer of 1 dense unit giving a parameter of 51 (2nd layer + output layer). This gives a total parameter of 7,621. This volume was set to try optimize up to 75% accuracy of the model.
    ![image](https://user-images.githubusercontent.com/78067427/123915595-ac84e880-d94e-11eb-95ce-a153b54cfb7f.png)
    
   - The model's performance was not able to reach a 75% accuracy level 
    ![image](https://user-images.githubusercontent.com/78067427/123918421-dbe92480-d951-11eb-9ef8-a802c670131a.png)
    
   - Further steps was taken to increase the nodes by overa 100%, additional layer added, different activation fumctions were used and the epochs was increased as well.
    ![image](https://user-images.githubusercontent.com/78067427/123919343-d9d39580-d952-11eb-856d-50ded3d3baba.png)
    ![image](https://user-images.githubusercontent.com/78067427/123919641-2028f480-d953-11eb-97d5-ab6652f9167c.png)

## Summary

For the most part, the model was retrained on several attempts but still gives about 72% accuracy level. 

It could be optimized better if more features are added, which may be related to the expenditures of the funding and other relevant information to be added to the dataset. Also, supervised learning model like Random Forest Classifier can be used to derive a categorized output and perhaps give a better accuracy performance.



   
   
