Deep Learning Challenge

Alphabet Soup performance of the deep learning model report

Overview of the analysis: 

 The purpose of the analysis is to use the neural network tool in selecting the applicants of Alphabet Soup for funding their ventures with the best chance of success. The features in the dataset provided were used to create a binary classifier in predicting if applicants will be successful if funded.


Data Preprocessing:
- In first attempt, "EIN" and "NAME" columns were dropped as this does not offer relevant data and help model to do better, and determined that the target variable is "IS_SUCCESSFUL"
-the rest of the columns were used as features

Compiling, Training, and Evaluating the Model:

- In first attempt, neural network consists of 80 neurons for first layer, 30 in second. Used relu activation for both layers, sigmoid for the output layer 
 was used. In nonlinear data, relu do better. Please see layer1 images in images folder.
- Performance metrics for first attempt is less than 75% which is 72.85%. Please see Evaluation1 image in images folder.
- To increase model performance, the "NAME" column was added back. First layer was changed from 80 to 7, the second layer was 14 from 30. Third layer was added with 21 neurons. The third layer was added to reweight inputs from the second layer
-  In optimization, I add back the "NAME" column. Changed the first layer from 80 to 7 neurons, the second layer from 30 to 14 neurons, also added a third layer with 21 neurons. By adding a third layer, I wanted to give the model another chance to reweight the inputs from the second layer to the third. The accuracy of more than 75% was achieved now. It's 78.49%
    
Results:
   - First attempt, the accuracy is 72.85%
   - In Optimized, the accuracy is 78.49%
   - 
Summary:
   From the analysis result, deep neural network helps come up a moderate useful binary classifier to predict if applicants will be successful for funding. 
   After the optimization test, the accuracy improved more than 75% to 78.49%. This was made by adding back the "NAME" column. The shape of the dataset is crucial before preprocessing.
  
