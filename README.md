CNN for Image Classification on MNIST Dataset
This CNN is created to classify the handwritten images of digits 0-9 in the MNIST dataset. The neural network is defined to identify the handwritten digits into 10 classes. 
I/P :- MNIST dataset. 
O/P :- 10 classes.

## MNIST dataset 
MNIST is a dataset of handwritten digits from 0-9.


![image](https://github.com/ShikhaERAV2/Session6/assets/160948226/ca4b764d-2776-4776-bf7c-67fe1f9163ff)

## Model Description
This is a Multiple  convolution layers in Convolutional Neural Network for digits identification trained on MNIST dataset. Added dropout and batch normalization to improve the accuracy of the model.
Batch normalization is added after couple of convolution layers and Dropout is added away from the last layer. Addition to the above steps Image Augmentation is used to improve model accuracy and overfitting problem. Finally Learning Rate has been changed to imporve the models accuracy and find the best learning rate. 

## Code Structure 
- `S7_Model_1.ipynb`: The main Jupyter Notebook contains the code to load data in train and test datasets -> transform data-> load model (defined in model.py)-> train  model -> test the model -> Check the accuracy of the model thus trained.
- `S7_Model_2.ipynb`: The main Jupyter Notebook contains the code to load data in train and test datasets -> transform data-> load model (defined in model.py)-> train  model -> test the model -> Check the accuracy of the model thus trained.
- `S7_Model_3.ipynb`: The main Jupyter Notebook contains the code to load data in train and test datasets -> transform data-> load model (defined in model.py)-> train  model -> test the model -> Check the accuracy of the model thus trained. 
- `model.py`: This file contains the definition of the model. Basic architecture of the model is defined with multiple convolution layers and fully connected layers. 
- `utils.py`: This file contains the utility functions like display of the sample data images and plotting the accuracy and loss during training. 

## Requirements
- Pytorch
- Matplotlib

## Model 1 - Experiment 1
Model Name : Net1

*Test Accuracy = 99.3% (max)

*Train Accuracy = 99.7%

*Total params: 15,580

Analysis:

1. Model is overfitting.
2. Number of parameter is less though but model can perform better.
3. Added one more convolution layer
4. changed the number of channels on the model

## Model 1- Experiment 2
Model Name : Net2 

*Test Accuracy = 99.22% (max)

*Train Accuracy = 99.56%

*Total params: 12,704

Analysis:

1.Increasing the conv layer but reducing the number of channels in the output layer
2. Model is still over fitting. 

## Model 1- Final
Model Name : Net

*Test Accuracy = 99.20% (max)

*Train Accuracy = 99.36%

*Total params: 7,596

Analysis:

1. Model is slightly overfitting.
2.  As the number of epoch increases the model training is moving towards overfitting.
3.  Though model parameter count is pretty small.

![image](https://github.com/ShikhaERAV2/Session7/assets/160948226/43067b31-79ae-4147-a376-c8258d5ee401)


## Model 2

Model name : Net 

Results:

*Best Train Accuracy: 98.99%

*Best Test Accuracy: 99.26%

*Parameters: 7,596

Analysis:

1. Updating the Image augmentation to check the impact on model accuracy.
2. Augmentation technique of rotation is used.
3. Tried augmenting using color gitter and crop but didnt give good accuracy. 
4. Model is Underfitting.

![image](https://github.com/ShikhaERAV2/Session7/assets/160948226/cab91958-7120-4857-94f1-d139d70d6b28)


## Model 3 

*Best Train Accuracy: 99.16%

*Best Test Accuracy:  99.45%

*Parameters: 7,596

Analysis:
1. Model is underfitting.
2. The accuracy has reached the 99.45% with the experiment in the Learning rate using the StepLR. 

![image](https://github.com/ShikhaERAV2/Session7/assets/160948226/092a5c29-c4ce-46b7-ad50-8ecf914ac35d)



