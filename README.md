# Deep Learning Homework: Charity Funding Predictor


**Overview**
* Purpose is to create a model to predict if the companies funded by the AlphabetSoup organization will be successful.

**Results**
* PreProcessing Details

* IS_SUCCESSFUL is the column/field used as target for the model.
      
* The below columns are considered as the features for the model.

    - APPLICATION_TYPE            
    - AFFILIATION                  
    - CLASSIFICATION              
    - USE_CASE                     
    - ORGANIZATION                 
    - STATUS                       
    - INCOME_AMT                   
    - SPECIAL_CONSIDERATIONS       
    - ASK_AMT
    

* The columns EIN, NAME are removed from the data as those are not targets or features to be considered
    
* For the neural network model, 

   - Two hidden layers are used. 
   - First with 7 neurons , second with 14 neurons. 
   - relu is the activation function used to get an ouput of min of 0 and going upward.

           - hidden_nodes_layer1=7    
           - hidden_nodes_layer2=14
 
            -nn.add(tf.keras.layers.Dense(units=hidden_nodes_layer1, input_dim=number_input_features, activation='relu'))

            -nn.add(tf.keras.layers.Dense(units=hidden_nodes_layer2, activation='relu'))


* The target model has

    - Accuracy: 0.7303789854049683
    - Model has an accuracy of 0.7303
    
* Added another hidden layer to improve the accuracy, but was not able to get to 75% .
* Changed the number of neurons to improve the performance.
* Increased the number of epochs to 200  and tried to improve the accuracy.

