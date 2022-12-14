# Determine-the-Diabetes-Disease-with-Neural-Network
# Executive Summary  
## About the Dataset      

* I used Pima Indian Diabetes dataset from Kaggle.      
* There are 768 people data and 9 characteristics which is one of them classification column.   

## Data Preprocessing      

* There are no missing values.      
* I used Min-Max Scaler to prevent the biased results.      
* I splitted data 20% test 80% train.      
* Also, I used Shuffle True, while dividing data.   

## Build the Model      

* I built a neural network by using Tensorflow and Keras.     
* I used Sequential API while building my model.     
* At the begining of my analysis I implement three layers with one hidden layer.      
* I used 15 perceptron the first layer and hidden layer.      
* I defined 1 output layer.      
* I stated ReLu activation function on the input and hidden layer, and sigmoid activation function on the output layer.      
* I used Adam as a optimizer and, Binary Crossentropy for loss, and accuracy metric. I used 1000 epoch and 57 batch size.  

## Evaluate the Model     

* Unfortunately, my model caused over-fitting.      
* The model had a high accuracy on the train dataset, however had a low accuracy on the test dataset.     
* Firstly, To prevent the overfitting, I decrease epoch size from 1000 to 500. But it couldn't work.     
* Secondly, I decrease batch size  from 57 to 16. I reached the same result.     
* Thirdly, I added Dropout Layer with 0.2 dropout rate.     
* Finally, I can reach reliable and aceptable model acuracy both of them (train, test dataset) which train accuracy was 0.79 and test accuracy was .77.     
* I added the plot of the train and test loss and accuracy at the end of the project.
