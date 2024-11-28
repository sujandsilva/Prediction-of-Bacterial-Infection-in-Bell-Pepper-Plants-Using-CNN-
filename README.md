# Prediction-of-Bacterial-Infection-in-Bell-Pepper-Plants-Using-CNN-
In this project, I have implemented a CNN architechture using keras library of tensorflow to identify bacterial infections in bell pepper leaves, achieving an accuracy of 99%                                 
1. Images belonging to 2 classes ('Healthy' and 'Bacterial_spot' were imported from directory followed by resizing and shuffling
2. The CNN architechture is as follows:
   1st Layer - 'resize and rescale' to resize the images to 256 * 256 and normalize the pixel values
   2nd Layer - 'data augmentation': randomly flipping and rotating the images to increase generalization
   3rd - 8th Layers - 6 Convolution layers with (3,3) filters and 'relu' activation followed by MaxPooling layers
   9th Layer - Flatten: input layer to the fully connected layer
   10th - 11th Layers - 1 hidden layer with 'relu' activation and 1 output layer with 'softmax'
3. Around 200,000 parameters trained by the network
4. Used EarlyStopping to reduce the chances of overfitting and divergence during training\
5. Achieved an accuarcy of 99% afer the training
6. Created a 'predict' function to take model and image as input and render the class and confidence as the output                                               
Dataset: https://www.kaggle.com/datasets/abdallahalidev/plantvillage-dataset
